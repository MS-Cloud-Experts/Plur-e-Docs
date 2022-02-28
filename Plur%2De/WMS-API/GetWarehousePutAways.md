**ProcessMethod**: GetWarehousePutAways

**Description**:
This method returns the elements of the table "**Warehouse Activity Header**" filtered so that only "**Put-Away**" is visible. In this case, the filtered record is brought in the "No" field. returning the "**Warehouse Activity Header**" in JSON format.

**Input**:

**Parameters**: 
-	**assigned_user_id**: filter that allows obtaining only the warehouse put-aways of a user. If it is left blank, it brings all the existing ones.

**Ouput**:  

-	**WarehousePutAways**: Contains an array of Warehouse Activity Header of type Put-Away in expressed in the key WarehousePutAways

**Example**:

**Request**:

 `"jsonRequest":"{\"ProcessMethod\":\"GetWarehousePutAways\",\"Parameters\":[{\"assigned_user_id\":\"\"}]}"`

**Outputs**:

**WarehousePutAways:**
![image.png](/.attachments/image-e2484987-eff5-4498-90dc-7cfc8267a48f.png)

```
{
  "WarehousePutAways": [
    {
      "id": 5766,
      "name": "WarehouseActivityHeader",
      "company": "CRONUS USA, Inc.",
      "position": "Type=CONST(Put-away),No.=CONST(10112)",
      "recordId": "Warehouse Activity Header: Put-away,10112",
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
            "value": 10112,
            "System": "false"
          }
        ]
      },
      "fieldCount": 33,
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
          "value": 10112,
          "System": "false"
        },
        {
          "id": 3,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": "false"
        },
        {
          "id": 4,
          "name": "AssignedUserID",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 5,
          "name": "AssignmentDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 6,
          "name": "AssignmentTime",
          "type": "Time",
          "value": null,
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
          "id": 12,
          "name": "NoPrinted",
          "type": "Integer",
          "value": null,
          "System": "false"
        },
        {
          "id": 13,
          "name": "NoofLines",
          "type": "Integer",
          "value": 6,
          "System": "false"
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 61,
          "name": "RegisteringNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 62,
          "name": "LastRegisteringNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 63,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": "PICK",
          "System": "false"
        },
        {
          "id": 7303,
          "name": "DateofLastPrinting",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 7304,
          "name": "TimeofLastPrinting",
          "type": "Time",
          "value": null,
          "System": "false"
        },
        {
          "id": 7305,
          "name": "BreakbulkFilter",
          "type": "Boolean",
          "value": "false",
          "System": "false"
        },
        {
          "id": 7306,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 7307,
          "name": "SourceDocument",
          "type": "Option",
          "value": " ",
          "System": "false"
        },
        {
          "id": 7308,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": "false"
        },
        {
          "id": 7309,
          "name": "SourceSubtype",
          "type": "Option",
          "value": 0,
          "System": "false"
        },
        {
          "id": 7310,
          "name": "DestinationType",
          "type": "Option",
          "value": " ",
          "System": "false"
        },
        {
          "id": 7311,
          "name": "DestinationNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 7312,
          "name": "ExternalDocumentNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 7313,
          "name": "ExpectedReceiptDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 7314,
          "name": "ShipmentDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 7315,
          "name": "ExternalDocumentNo2",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{52D2F71F-5D96-EC11-80F2-000D3A74F81B}",
          "System": "false"
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-25T17:05:26.8930000Z",
          "System": "false"
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": "false"
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-02-25T17:05:26.8930000Z",
          "System": "false"
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": "false"
        }
      ]
    }
  ]
}
```


`"{"Error":"The Warehouse Activity List is Empty"}"`

