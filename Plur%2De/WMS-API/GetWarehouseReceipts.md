**ProcessMethod**: GetWarehouseReceipts

**Description**:
Allows you to bring a list of open Warehouse Receipts to be posted in a Warehouse Activity (Warehouse Put-Away) or assign a License Plate.

**Parameters**: 

**Input**:

**Parameters**: 
-	**assigned_user_id**: filter that allows obtaining only the warehouse receipts of a user. If it is left blank, it brings all the existing ones.

**Ouput**: Returns an array of Warehouse Receipts in Json format.

-	**WarehouseReceipts**: Returns an array of Warehouse Receipts expressed in the key: `WarehouseReceipts`

**Example**:

**Request:**
`"jsonRequest":"{"ProcessMethod":"GetWarehouseReceipts","Parameters":[{"assigned_user_id":""}]}"`

**Error**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Receipt List is Empty."
  }
}
```
**Output**:

**WarehouseReceipts:**

![image.png](/.attachments/image-eaca9fc1-e4fe-46d1-86ad-2b28cb94e452.png)

**Output:**

```
{
  "WarehouseReceipts": [
    {
      "id": 7316,
      "name": "WarehouseReceiptHeader",
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(107292)",
      "recordId": "Warehouse Receipt Header: 107292",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 1,
            "name": "No",
            "type": "Code",
            "value": "107292",
            "System": false
          }
        ]
      },
      "fieldCount": 24,
      "fields": [
        {
          "id": 1,
          "name": "No",
          "type": "Code",
          "value": "107292",
          "System": false
        },
        {
          "id": 2,
          "name": "LocationCode",
          "type": "Code",
          "value": "ADVANCED1",
          "System": false
        },
        {
          "id": 3,
          "name": "AssignedUserID",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 4,
          "name": "AssignmentDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 5,
          "name": "AssignmentTime",
          "type": "Time",
          "value": null,
          "System": false
        },
        {
          "id": 6,
          "name": "SortingMethod",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 7,
          "name": "NoSeries",
          "type": "Code",
          "value": "P-RCPT",
          "System": false
        },
        {
          "id": 8,
          "name": "ZoneCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 9,
          "name": "BinCode",
          "type": "Code",
          "value": "REC",
          "System": false
        },
        {
          "id": 10,
          "name": "DocumentStatus",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 11,
          "name": "Comment",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 12,
          "name": "PostingDate",
          "type": "Date",
          "value": "2022-02-04",
          "System": false
        },
        {
          "id": 13,
          "name": "VendorShipmentNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 16,
          "name": "CrossDockZoneCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 17,
          "name": "CrossDockBinCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "CreatePostedHeader",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 51,
          "name": "ReceivingNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 62,
          "name": "LastReceivingNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 63,
          "name": "ReceivingNoSeries",
          "type": "Code",
          "value": "PWHSRCPT",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{217508CD-EB93-EC11-B85A-000D3A722756}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-22T14:29:11.827Z",
          "System": false
        },
        
      ]
    }
  ]
}
```

