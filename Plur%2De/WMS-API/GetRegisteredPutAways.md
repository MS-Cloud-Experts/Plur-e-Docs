**ProcessMethod**: GetRegisteredPutAways

**Description**:
This method returns the elements of the table "Registered Whse. Activity Hdr." filtered so that only "Registered Put-Away" is visible. In this case, the filtered record is brought in the "No" field. returning the "Registered Whse. Activity Hdr" and the "Registered Whse. Activity Line" in JSON format.

**Input**:

**Parameters**: 
-	**assigned_user_id**: filter that allows obtaining only the warehouse receipts of a user. If it is left blank, it brings all the existing ones.

**Ouput**:  

-	**RegisteredPutAways**: Contains an array of `RegisteredPutAways` in the key: `RegisteredWhseActivityHdr`.

**Example**:

**RegisteredPutAways:** 

The following image shows the Warehouse Put-Aways registered using filter.

![image.png](/.attachments/image-026b253b-c368-452f-9791-e28b41970178.png)

**RegisteredPutAways:**
![image.png](/.attachments/image-f09e0815-5c59-4f7f-93d3-0eff33d43537.png)

**Request:**

    "jsonRequest":"{\"ProcessMethod\":\"GetRegisteredPutAways\",\"Parameters\":[{\"assigned_user_id\":\"\"}]}"

**Outputs**:

```
{
  "RegisteredPutAways": [
    {
      "id": 5772,
      "name": "RegisteredWhseActivityHdr",
      "company": "CRONUS USA, Inc.",
      "position": "Type=CONST(Put-away),No.=CONST(10095)",
      "recordId": "Registered Whse. Activity Hdr.: Put-away,10095",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "Type",
            "type": "Option",
            "value": "Put-away",
            "System": "false"
          },
          {
            "id": 2,
            "name": "No",
            "type": "Code",
            "value": 10095,
            "System": "false"
          }
        ]
      },
      "fieldCount": 17,
      "fields": [
        {
          "id": 1,
          "name": "Type",
          "type": "Option",
          "value": "Put-away",
          "System": "false"
        },
        {
          "id": 2,
          "name": "No",
          "type": "Code",
          "value": 10095,
          "System": "false"
        },
        {
          "id": 3,
          "name": "LocationCode",
          "type": "Code",
          "value": "MAIN WMS",
          "System": "false"
        },
        {
          "id": 4,
          "name": "AssignedUserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": "false"
        },
        {
          "id": 5,
          "name": "AssignmentDate",
          "type": "Date",
          "value": "2022-02-23",
          "System": "false"
        },
        {
          "id": 6,
          "name": "AssignmentTime",
          "type": "Time",
          "value": "11:59:27.35",
          "System": "false"
        },
        {
          "id": 7,
          "name": "SortingMethod",
          "type": "Option",
          "value": " ",
          "System": "false"
        },
        {
          "id": 8,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-02-04",
          "System": "false"
        },
        {
          "id": 9,
          "name": "NoSeries",
          "type": "Code",
          "value": "PICK",
          "System": "false"
        },
        {
          "id": 10,
          "name": "Comment",
          "type": "Boolean",
          "value": "false",
          "System": "false"
        },
        {
          "id": 11,
          "name": "WhseActivityNo",
          "type": "Code",
          "value": 10093,
          "System": "false"
        },
        {
          "id": 12,
          "name": "NoPrinted",
          "type": "Integer",
          "value": null,
          "System": "false"
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{1DD2C94F-C294-EC11-80F2-000D3A74F212}",
          "System": "false"
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-23T16:04:43.6400000Z",
          "System": "false"
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
          "System": "false"
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-02-23T16:04:43.6400000Z",
          "System": "false"
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
          "System": "false"
        }
      ]
    }
  ]
}
```


**Errors**:


```
{
  "Error": {
    "Code": "Not found",
    "Message": The Registered Whse. Activity Hdr. not exist"
  }
}
```


