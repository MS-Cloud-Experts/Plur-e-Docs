**Item Tracking Lines Open:**

![image.png](/.attachments/image-723d75d5-d765-4c0c-8e3c-f6362c9721ff.png)

**Item Tracking:**

![image.png](/.attachments/image-5918d26f-6798-47ce-ab89-1fa604a2f02a.png)

![image.png](/.attachments/image-45d7e8d5-1bc4-4bf7-9b3a-571922e61f0b.png)

**Input**

```
{
  "ProcessMethod": "GetItemTrackingSpecificationV2",
  "Parameters": [
    {
      "ItemNo": "1000",
      "SourceNo": "106014",
      "SourceRefNo": "20000"
    }
  ]
}
```


**OutPut**

```
{
  "ItemTrackingOpenJO": {
    "TrackingSpecificationOpen": [
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(859),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 859,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 859,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 859,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I10",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01181",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Single",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{BB058DD6-E6D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:19:52.4800000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:19:52.5900000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(860),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 860,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 860,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 860,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I11",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01181",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Single",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{BC058DD6-E6D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:19:52.4970000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:19:52.5900000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(861),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 861,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 861,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 861,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I12",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01182",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Single",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{A25FBAE2-E6D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:22.6770000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:22.6900000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(862),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 862,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 862,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 862,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I13",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01182",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Single",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{A35FBAE2-E6D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:22.6770000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:22.6900000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(863),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 863,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 863,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 863,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I14",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01183",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Single",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{5ABE18F5-E6D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:49.1970000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:49.2130000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(864),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 864,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 864,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 864,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I15",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01183",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Single",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{5BBE18F5-E6D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:49.1970000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:20:49.2130000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(865),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 865,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 865,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 865,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I16",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01184",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Pallet",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{7309A338-E7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:22:39.6970000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:22:39.8200000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(866),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 866,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 866,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 866,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I17",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01184",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Pallet",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{7409A338-E7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:22:39.6970000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:22:39.8200000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(867),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 867,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 867,
              "System": false
            },
            {
              "id": 28,
              "name": "Positive",
              "type": "Boolean",
              "value": true,
              "System": false
            }
          ]
        },
        "fieldCount": 52,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 867,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1013",
            "System": false
          },
          {
            "id": 3,
            "name": "LocationCode",
            "type": "Code",
            "value": "NEWWMS",
            "System": false
          },
          {
            "id": 4,
            "name": "QuantityBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 5,
            "name": "ReservationStatus",
            "type": "Option",
            "value": "Surplus",
            "System": false
          },
          {
            "id": 7,
            "name": "Description",
            "type": "Text",
            "value": null,
            "System": false
          },
          {
            "id": 8,
            "name": "CreationDate",
            "type": "Date",
            "value": "2023-04-05",
            "System": false
          },
          {
            "id": 9,
            "name": "TransferredfromEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 10,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": false
          },
          {
            "id": 11,
            "name": "SourceSubtype",
            "type": "Option",
            "value": "1",
            "System": false
          },
          {
            "id": 12,
            "name": "SourceID",
            "type": "Code",
            "value": "106178",
            "System": false
          },
          {
            "id": 13,
            "name": "SourceBatchName",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "SourceProdOrderLine",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "SourceRefNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          },
          {
            "id": 16,
            "name": "ItemLedgerEntryNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 22,
            "name": "ExpectedReceiptDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 23,
            "name": "ShipmentDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 24,
            "name": "SerialNo",
            "type": "Code",
            "value": "I18",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "INTEGRATION WITH PLUR-E APP",
            "System": false
          },
          {
            "id": 27,
            "name": "ChangedBy",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 28,
            "name": "Positive",
            "type": "Boolean",
            "value": true,
            "System": false
          },
          {
            "id": 29,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 30,
            "name": "Quantity",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 31,
            "name": "ActionMessageAdjustment",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 32,
            "name": "Binding",
            "type": "Option",
            "value": " ",
            "System": false
          },
          {
            "id": 33,
            "name": "SuppressedActionMsg",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 34,
            "name": "PlanningFlexibility",
            "type": "Option",
            "value": "Unlimited",
            "System": false
          },
          {
            "id": 38,
            "name": "AppltoItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 40,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 41,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 50,
            "name": "QtytoHandleBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 53,
            "name": "QuantityInvoicedBase",
            "type": "Decimal",
            "value": null,
            "System": false
          },
          {
            "id": 80,
            "name": "NewSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 81,
            "name": "NewLotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 900,
            "name": "DisallowCancellation",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 5400,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5401,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 5811,
            "name": "ApplfromItemEntry",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 5817,
            "name": "Correction",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6505,
            "name": "NewExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 6510,
            "name": "ItemTracking",
            "type": "Option",
            "value": "Serial No.",
            "System": false
          },
          {
            "id": 6511,
            "name": "UntrackedSurplus",
            "type": "Boolean",
            "value": false,
            "System": false
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6516,
            "name": "NewPackageNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 71017575,
            "name": "PLULPDocumentNo",
            "type": "Code",
            "value": "LP-01184",
            "System": false
          },
          {
            "id": 71017576,
            "name": "PLULPDocumentType",
            "type": "Option",
            "value": "Pallet",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{7509A338-E7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:22:39.6970000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T19:22:39.8200000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
            "System": false
          }
        ]
      }
    ]
  },
  "ItemTrackinCloseJO": {
    "Error": "The TrackingSpecification ItemNo does not exist."
  },
  "ItemTrackingJO": {
    "ItemTracking": {
      "id": 6502,
      "name": "ItemTrackingCode",
      "company": "CRONUS USA, Inc.",
      "position": "Code=CONST(SNALLWH)",
      "recordId": "Item Tracking Code: SNALLWH",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 1,
            "name": "Code",
            "type": "Code",
            "value": "SNALLWH",
            "System": false
          }
        ]
      },
      "fieldCount": 65,
      "fields": [
        {
          "id": 1,
          "name": "Code",
          "type": "Code",
          "value": "SNALLWH",
          "System": false
        },
        {
          "id": 2,
          "name": "Description",
          "type": "Text",
          "value": null,
          "System": false
        },
        {
          "id": 3,
          "name": "WarrantyDateFormula",
          "type": "DateFormula",
          "value": null,
          "System": false
        },
        {
          "id": 5,
          "name": "ManWarrantyDateEntryReqd",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 6,
          "name": "ManExpirDateEntryReqd",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 8,
          "name": "StrictExpirationPosting",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 9,
          "name": "UseExpirationDates",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 11,
          "name": "SNSpecificTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 13,
          "name": "SNInfoInboundMustExist",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 14,
          "name": "SNInfoOutboundMustExist",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 15,
          "name": "SNWarehouseTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 21,
          "name": "SNPurchaseInboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 22,
          "name": "SNPurchaseOutboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 23,
          "name": "SNSalesInboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 24,
          "name": "SNSalesOutboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 25,
          "name": "SNPosAdjmtInbTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 26,
          "name": "SNPosAdjmtOutbTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 27,
          "name": "SNNegAdjmtInbTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 28,
          "name": "SNNegAdjmtOutbTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 29,
          "name": "SNTransferTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 30,
          "name": "SNManufInboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 31,
          "name": "SNManufOutboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 32,
          "name": "SNAssemblyInboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 33,
          "name": "SNAssemblyOutboundTracking",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 34,
          "name": "CreateSNInfoonPosting",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 41,
          "name": "LotSpecificTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 43,
          "name": "LotInfoInboundMustExist",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 44,
          "name": "LotInfoOutboundMustExist",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 45,
          "name": "LotWarehouseTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 51,
          "name": "LotPurchaseInboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 52,
          "name": "LotPurchaseOutboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 53,
          "name": "LotSalesInboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 54,
          "name": "LotSalesOutboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 55,
          "name": "LotPosAdjmtInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 56,
          "name": "LotPosAdjmtOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 57,
          "name": "LotNegAdjmtInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 58,
          "name": "LotNegAdjmtOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 59,
          "name": "LotTransferTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 60,
          "name": "LotManufInboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 61,
          "name": "LotManufOutboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 62,
          "name": "LotAssemblyInboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 63,
          "name": "LotAssemblyOutboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 64,
          "name": "CreateLotNoInfoonposting",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 70,
          "name": "PackageSpecificTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 71,
          "name": "PackageWarehouseTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 73,
          "name": "PackageInfoInbMustExist",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 74,
          "name": "PackageInfoOutbMustExist",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 75,
          "name": "PackagePurchaseInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 76,
          "name": "PackagePurchOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 77,
          "name": "PackageSalesInboundTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 78,
          "name": "PackageSalesOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 79,
          "name": "PackagePosInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 80,
          "name": "PackagePosOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 81,
          "name": "PackageNegInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 82,
          "name": "PackageNegOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 83,
          "name": "PackageTransferTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 84,
          "name": "PackageManufInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 85,
          "name": "PackageManufOutbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 86,
          "name": "PackageAssemblyInbTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 87,
          "name": "PackageAssemblyOutTracking",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{EFC711E2-ACAC-ED11-9A8A-6045BD3623CE}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2023-02-14T21:16:46.8170000Z",
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
          "value": "2023-02-14T21:16:49.1000000Z",
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
    }
  }
}
  

```



**Errors**

```
{
  "Error": "The TrackingSpecification does not exist.",
  "ItemIdentifier": [
    {
      "Code": "",
      "VariantCode": "",
      "UnitofMeasureCode": ""
    }
  ]
}
```
