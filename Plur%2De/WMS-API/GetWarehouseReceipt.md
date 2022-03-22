**ProcessMethod**: GetWarehouseReceipt

**Description**: It allows to bring a particular Warehouse Receipt through the key field No.

**Input:**
**Parameters:** 
-	**No**: Allows you to bring a single Warehouse Receipt.


**Ouput**: 

**WarehouseReceipt**: Contains a `WarehouseReceiptHeader` and an array of lines expressed in the key: `WarehouseReceiptLines`.

**Example**:

**WarehouseReceiptHeader:**
![image.png](/.attachments/image-4c6fbc05-796d-4fce-8911-d445960b7df5.png)

**WarehouseReceiptLines:**
![image.png](/.attachments/image-4cb6d09d-97f3-4b31-95a4-e51c215a9b09.png)

**Request:**
`"jsonRequest":"{"ProcessMethod":"GetWarehouseReceipt","Parameters":[{"No":"107292"}]}"`

**Error**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Receipt does not exist."
  }
}
```


**Output**:

```
{
  "WarehouseReceipt": {
    "WarehouseReceiptHeader": {
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
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-02-22T14:29:11.827Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": false
        }
      ]
    },
    "WarehouseReceiptLines": [
      {
        "id": 7317,
        "name": "WarehouseReceiptLine",
        "company": "CRONUS USA, Inc.",
        "position": "No.=CONST(107292),Line No.=CONST(10000)",
        "recordId": "Warehouse Receipt Line: 107292,10000",
        "primaryKey": {
          "fieldCount": 2,
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
              "name": "LineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            }
          ]
        },
        "fieldCount": 47,
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
            "name": "LineNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 3,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 4,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 6,
            "name": "SourceNo",
            "type": "Code",
            "value": "106032",
            "System": false
          },
          {
            "id": 7,
            "name": "SourceLineNo",
            "type": "Integer",
            "value": 20000,
            "System": false
          },
          {
            "id": 9,
            "name": "SourceDocument",
            "type": "Option",
            "value": "Purchase Order",
            "System": false
          },
          {
            "id": 10,
            "name": "LocationCode",
            "type": "Code",
            "value": "ADVANCED1",
            "System": false
          },
          {
            "id": 11,
            "name": "ShelfNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 12,
            "name": "BinCode",
            "type": "Code",
            "value": "REC",
            "System": false
          },
          {
            "id": 13,
            "name": "ZoneCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "ItemNo",
            "type": "Code",
            "value": "100A",
            "System": false
          },
          {
            "id": 15,
            "name": "Quantity",
            "type": "Decimal",
            "value": 10.0,
            "System": false
          },
          {
            "id": 16,
            "name": "Qty(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": false
          },
          {
            "id": 19,
            "name": "QtyOutstanding",
            "type": "Decimal",
            "value": 10.0,
            "System": false
          },
          {
            "id": 20,
            "name": "QtyOutstanding(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": false
          },
          {
            "id": 21,
            "name": "QtytoReceive",
            "type": "Decimal",
            "value": 10.0,
            "System": false
          },
          {
            "id": 22,
            "name": "QtytoReceive(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": false
          },
          {
            "id": 23,
            "name": "QtyReceived",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "QtyReceived(Base)",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 29,
            "name": "UnitofMeasureCode",
            "type": "Code",
            "value": "PCS",
            "System": false
          },
          {
            "id": 30,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Description",
            "type": "Text",
            "value": "100A",
            "System": false
          },
          {
            "id": 33,
            "name": "Description2",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 34,
            "name": "Status",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 35,
            "name": "SortingSequenceNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 36,
            "name": "DueDate",
            "type": "Date",
            "value": "2022-02-04",
            "System": false
          },
          {
            "id": 37,
            "name": "StartingDate",
            "type": "Date",
            "value": "2022-02-04",
            "System": false
          },
          {
            "id": 38,
            "name": "Cubage",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 39,
            "name": "Weight",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 48,
            "name": "NotupdbySrcDocPost",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 49,
            "name": "PostingfromWhseRef",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoCrossDock",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoCrossDock(Base)",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 52,
            "name": "CrossDockZoneCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 53,
            "name": "CrossDockBinCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 55,
            "name": "QtyRoundingPrecision",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 56,
            "name": "QtyRoundingPrecision(Base)",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 8509,
            "name": "OverReceiptQuantity",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 8510,
            "name": "OverReceiptCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLUNoLPCreated",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{227508CD-EB93-EC11-B85A-000D3A722756}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2022-02-22T14:29:11.843Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2022-02-22T14:29:11.843Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": false
          }
        ]
      }
    ]
  }
}
```


