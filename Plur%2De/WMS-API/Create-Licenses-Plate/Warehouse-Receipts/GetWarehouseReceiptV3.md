**ProcessMethod**: GetWarehouseReceiptV3

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
      "position": "No.=CONST(WHSE REC-00155)",
      "recordId": "Warehouse Receipt Header: WHSE REC-00155",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 1,
            "name": "No",
            "type": "Code",
            "value": "WHSE REC-00155",
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
          "value": "WHSE REC-00155",
          "System": false
        },
        {
          "id": 2,
          "name": "LocationCode",
          "type": "Code",
          "value": "NEWWMS",
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
          "value": "WHSE REC",
          "System": false
        },
        {
          "id": 8,
          "name": "ZoneCode",
          "type": "Code",
          "value": "REC",
          "System": false
        },
        {
          "id": 9,
          "name": "BinCode",
          "type": "Code",
          "value": "REC-1",
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
          "value": "2023-04-10",
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
          "value": "WHSE REC+",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{506FB393-F2D2-ED11-A7C9-000D3A9FD6E8}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2023-04-04T14:11:26.6530000Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{0081F62B-F63D-4697-8E47-82DBEA14BD9D}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2023-04-04T14:11:26.6530000Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{0081F62B-F63D-4697-8E47-82DBEA14BD9D}",
          "System": false
        }
      ]
    },
    "WarehouseReceiptLines": [
      {
        "No": "WHSE REC-00155",
        "LineNo": 10000,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106177",
        "SourceLineNo": 10000,
        "LocationCode": "NEWWMS",
        "BinCode": "REC-1",
        "ZoneCode": "REC",
        "ItemNo": "1013",
        "Quantity": 20.0,
        "QtyBase": 20.0,
        "QtyOutstanding": 20.0,
        "QtyOutstandingBase": 20.0,
        "QtytoReceive": 6.0,
        "QtytoReceiveBase": 6.0,
        "QtyReceived": 0.0,
        "QtyReceivedBase": 0.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "VariantCode": "",
        "OverReceiptQuantity": 0.0,
        "OverReceiptCode": "",
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "LPArray": {
          "LicensePlates": [
            {
              "LPDocumentNo": "LP-01173",
              "LPDocumentType": "Single",
              "LicensePlateStatus": "Received",
              "Location Code": "NEWWMS",
              "Bin Code": "REC-1",
              "WhseDocumentNo": "WHSE REC-00155",
              "UnitofMeasure": "PCS",
              "LPTotalQuantities": 0.0,
              "ItemNo": "",
              "LPLines": [
                {
                  "LPDocumentNo": "LP-01173",
                  "LPDocumentType": "Single",
                  "LineNo": 1000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "I1",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 1.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 10000
                },
                {
                  "LPDocumentNo": "LP-01173",
                  "LPDocumentType": "Single",
                  "LineNo": 2000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "I2",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 1.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 10000
                }
              ]
            },
            {
              "LPDocumentNo": "LP-01174",
              "LPDocumentType": "Single",
              "LicensePlateStatus": "Received",
              "Location Code": "NEWWMS",
              "Bin Code": "REC-1",
              "WhseDocumentNo": "WHSE REC-00155",
              "UnitofMeasure": "PCS",
              "LPTotalQuantities": 0.0,
              "ItemNo": "",
              "LPLines": [
                {
                  "LPDocumentNo": "LP-01174",
                  "LPDocumentType": "Single",
                  "LineNo": 1000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "I3",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 1.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 10000
                },
                {
                  "LPDocumentNo": "LP-01174",
                  "LPDocumentType": "Single",
                  "LineNo": 2000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "I4",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 1.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 10000
                }
              ]
            },
            {
              "LPDocumentNo": "LP-01175",
              "LPDocumentType": "Single",
              "LicensePlateStatus": "Received",
              "Location Code": "NEWWMS",
              "Bin Code": "REC-1",
              "WhseDocumentNo": "WHSE REC-00155",
              "UnitofMeasure": "PCS",
              "LPTotalQuantities": 0.0,
              "ItemNo": "",
              "LPLines": [
                {
                  "LPDocumentNo": "LP-01175",
                  "LPDocumentType": "Single",
                  "LineNo": 1000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "I5",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 1.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 10000
                },
                {
                  "LPDocumentNo": "LP-01175",
                  "LPDocumentType": "Single",
                  "LineNo": 2000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "I6",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 1.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 10000
                }
              ]
            }
          ]
        },
        "PLUNoLPCreated": 6.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "LP-01173|LP-01174|LP-01175",
        "PLULPPalletChildasItems": "",
        "PLUNewQtyOutstanding": 14.0
      },
      {
        "No": "WHSE REC-00155",
        "LineNo": 20000,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106177",
        "SourceLineNo": 20000,
        "LocationCode": "NEWWMS",
        "BinCode": "REC-1",
        "ZoneCode": "REC",
        "ItemNo": "1906-S",
        "Quantity": 12.0,
        "QtyBase": 12.0,
        "QtyOutstanding": 12.0,
        "QtyOutstandingBase": 12.0,
        "QtytoReceive": 12.0,
        "QtytoReceiveBase": 12.0,
        "QtyReceived": 0.0,
        "QtyReceivedBase": 0.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "VariantCode": "",
        "OverReceiptQuantity": 0.0,
        "OverReceiptCode": "",
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "",
        "LPArray": {
          "LicensePlates": [
            {
              "LPDocumentNo": "LP-01170",
              "LPDocumentType": "Single",
              "LicensePlateStatus": "Received",
              "Location Code": "NEWWMS",
              "Bin Code": "REC-1",
              "WhseDocumentNo": "WHSE REC-00155",
              "UnitofMeasure": "PCS",
              "LPTotalQuantities": 0.0,
              "ItemNo": "",
              "LPLines": [
                {
                  "LPDocumentNo": "LP-01170",
                  "LPDocumentType": "Single",
                  "LineNo": 20000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 3.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 20000
                }
              ]
            },
            {
              "LPDocumentNo": "LP-01171",
              "LPDocumentType": "Single",
              "LicensePlateStatus": "Received",
              "Location Code": "NEWWMS",
              "Bin Code": "REC-1",
              "WhseDocumentNo": "WHSE REC-00155",
              "UnitofMeasure": "PCS",
              "LPTotalQuantities": 0.0,
              "ItemNo": "",
              "LPLines": [
                {
                  "LPDocumentNo": "LP-01171",
                  "LPDocumentType": "Single",
                  "LineNo": 20000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 3.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 20000
                }
              ]
            },
            {
              "LPDocumentNo": "LP-01172",
              "LPDocumentType": "Single",
              "LicensePlateStatus": "Received",
              "Location Code": "NEWWMS",
              "Bin Code": "REC-1",
              "WhseDocumentNo": "WHSE REC-00155",
              "UnitofMeasure": "PCS",
              "LPTotalQuantities": 0.0,
              "ItemNo": "",
              "LPLines": [
                {
                  "LPDocumentNo": "LP-01172",
                  "LPDocumentType": "Single",
                  "LineNo": 20000,
                  "Type": "Item",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "ExpirationDate": "0001-01-01",
                  "Quantity": 3.0,
                  "QtyperUnitofMeasure": 1.0,
                  "SourceDocumentNo": "106177",
                  "SourceLineNo": 20000
                }
              ]
            }
          ]
        },
        "PLUNoLPCreated": 12.0,
        "PLULPSingles": "LP-01170|LP-01171|LP-01172",
        "PLULPPalletChildsasLP": "LP-01170|LP-01171|LP-01172",
        "PLULPPalletChildasItems": "LP-01176",
        "PLUNewQtyOutstanding": 0.0
      }
    ]
  }
}
```


