**Request:**

```
{
  "ProcessMethod": "GetItemTrackingSpecificationV3",
  "Parameters": [
    {
      "LocationCode": "NEWWMS"
    }
  ]
}
```
`{
  "ItemTrackingOpenJO": {
    "TrackingSpecificationOpen": [
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(831),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 831,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 831,
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
            "value": 831,
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
            "value": "2023-03-17",
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
            "value": "106173",
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
            "value": 20000,
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
            "value": "109",
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
            "value": "LP-01119",
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
            "value": "{68E07BDF-D5C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T15:10:38.4870000Z",
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
            "value": "2023-03-17T15:10:38.5330000Z",
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
        "position": "Entry No.=CONST(832),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 832,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 832,
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
            "value": 832,
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
            "value": "2023-03-17",
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
            "value": "106173",
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
            "value": 20000,
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
            "value": "110",
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
            "value": "LP-01119",
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
            "value": "{69E07BDF-D5C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T15:10:38.4870000Z",
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
            "value": "2023-03-17T15:10:38.5500000Z",
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
        "position": "Entry No.=CONST(833),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 833,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 833,
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
            "value": 833,
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
            "value": "2023-03-17",
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
            "value": "106173",
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
            "value": 20000,
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
            "value": "112",
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
            "value": "LP-01120",
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
            "value": "{36F49986-D6C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T15:15:18.8630000Z",
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
            "value": "2023-03-17T15:15:18.9270000Z",
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
        "position": "Entry No.=CONST(834),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 834,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 834,
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
            "value": 834,
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
            "value": "2023-03-17",
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
            "value": "106173",
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
            "value": 20000,
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
            "value": "113",
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
            "value": "LP-01120",
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
            "value": "{37F49986-D6C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T15:15:18.8630000Z",
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
            "value": "2023-03-17T15:15:18.9270000Z",
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
        "position": "Entry No.=CONST(835),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 835,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 835,
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
            "value": 835,
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
            "value": "2023-03-17",
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
            "value": "106173",
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
            "value": 20000,
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
            "value": "114",
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
            "value": "LP-01121",
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
            "value": "{827325A1-D6C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T15:16:03.3970000Z",
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
            "value": "2023-03-17T15:16:03.4770000Z",
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
        "position": "Entry No.=CONST(836),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 836,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 836,
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
            "value": 836,
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
            "value": "2023-03-17",
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
            "value": "106173",
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
            "value": 20000,
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
            "value": "115",
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
            "value": "LP-01121",
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
            "value": "{837325A1-D6C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T15:16:03.3970000Z",
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
            "value": "2023-03-17T15:16:03.4930000Z",
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
        "position": "Entry No.=CONST(837),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 837,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 837,
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
            "value": 837,
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
            "value": "2023-03-17",
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
            "value": "106174",
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
            "value": "116",
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
            "value": "LP-01130",
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
            "value": "{9F2CD374-DEC4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T16:12:05.0130000Z",
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
            "value": "2023-03-17T16:12:05.0900000Z",
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
        "position": "Entry No.=CONST(838),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 838,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 838,
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
            "value": 838,
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
            "value": "2023-03-17",
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
            "value": "106174",
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
            "value": "117",
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
            "value": "LP-01130",
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
            "value": "{A02CD374-DEC4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T16:12:05.0130000Z",
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
            "value": "2023-03-17T16:12:05.1070000Z",
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
        "position": "Entry No.=CONST(839),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 839,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 839,
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
            "value": 839,
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
            "value": "2023-03-17",
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
            "value": "106174",
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
            "value": "120",
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
            "value": "LP-01131",
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
            "value": "{02B687F6-E3C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T16:51:30.1070000Z",
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
            "value": "2023-03-17T16:51:30.3400000Z",
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
        "position": "Entry No.=CONST(840),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 840,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 840,
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
            "value": 840,
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
            "value": "2023-03-17",
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
            "value": "106174",
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
            "value": "121",
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
            "value": "LP-01131",
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
            "value": "{03B687F6-E3C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T16:51:30.1200000Z",
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
            "value": "2023-03-17T16:51:30.3530000Z",
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
        "position": "Entry No.=CONST(841),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 841,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 841,
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
            "value": 841,
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
            "value": "2023-03-17",
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
            "value": "106174",
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
            "value": "122",
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
            "value": "LP-01132",
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
            "value": "{F703E0E9-F6C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T19:07:09.3130000Z",
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
            "value": "2023-03-17T19:07:09.4370000Z",
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
        "position": "Entry No.=CONST(842),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 842,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 842,
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
            "value": 842,
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
            "value": "2023-03-17",
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
            "value": "106174",
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
            "value": "123",
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
            "value": "LP-01132",
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
            "value": "{F803E0E9-F6C4-ED11-9A88-000D3A3EA2EF}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-03-17T19:07:09.3130000Z",
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
            "value": "2023-03-17T19:07:09.4530000Z",
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
        "position": "Entry No.=CONST(851),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 851,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 851,
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
            "value": 851,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I1",
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
            "value": "LP-01173",
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
            "value": "{C60137D1-F2D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:13:09.7300000Z",
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
            "value": "2023-04-04T14:13:09.7930000Z",
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
        "position": "Entry No.=CONST(852),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 852,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 852,
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
            "value": 852,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I2",
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
            "value": "LP-01173",
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
            "value": "{C70137D1-F2D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:13:09.7300000Z",
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
            "value": "2023-04-04T14:13:09.7930000Z",
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
        "position": "Entry No.=CONST(853),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 853,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 853,
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
            "value": 853,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I3",
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
            "value": "LP-01174",
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
            "value": "{97C878DF-F2D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:13:35.3070000Z",
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
            "value": "2023-04-04T14:13:35.3230000Z",
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
        "position": "Entry No.=CONST(854),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 854,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 854,
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
            "value": 854,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I4",
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
            "value": "LP-01174",
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
            "value": "{98C878DF-F2D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:13:35.3070000Z",
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
            "value": "2023-04-04T14:13:35.3230000Z",
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
        "position": "Entry No.=CONST(855),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 855,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 855,
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
            "value": 855,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I5",
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
            "value": "LP-01175",
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
            "value": "{08E506F5-F2D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:14:11.3930000Z",
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
            "value": "2023-04-04T14:14:11.4070000Z",
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
        "position": "Entry No.=CONST(856),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 856,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 856,
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
            "value": 856,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I6",
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
            "value": "LP-01175",
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
            "value": "{09E506F5-F2D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:14:11.3930000Z",
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
            "value": "2023-04-04T14:14:11.4070000Z",
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
        "position": "Entry No.=CONST(857),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 857,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 857,
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
            "value": 857,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I7",
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
            "value": "LP-01176",
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
            "value": "{5570C224-F3D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:15:33.4330000Z",
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
            "value": "2023-04-04T14:15:33.4500000Z",
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
        "position": "Entry No.=CONST(858),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 858,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 858,
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
            "value": 858,
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
            "value": "2023-04-04",
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
            "value": "106177",
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
            "value": "I8",
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
            "value": "LP-01176",
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
            "value": "{5670C224-F3D2-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-04T14:15:33.4330000Z",
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
            "value": "2023-04-04T14:15:33.4500000Z",
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
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(868),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 868,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 868,
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
            "value": 868,
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
            "value": "106180",
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
            "value": "LP-01185",
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
            "value": "{ABBBCC92-F7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T21:19:49.7770000Z",
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
            "value": "2023-04-05T21:19:49.9200000Z",
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
        "position": "Entry No.=CONST(869),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 869,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 869,
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
            "value": 869,
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
            "value": "106180",
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
            "value": "LP-01185",
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
            "value": "{ACBBCC92-F7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T21:19:49.7930000Z",
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
            "value": "2023-04-05T21:19:49.9200000Z",
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
        "position": "Entry No.=CONST(870),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 870,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 870,
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
            "value": 870,
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
            "value": "106180",
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
            "value": "LP-01186",
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
            "value": "{ACCDEBB1-F7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T21:20:39.8700000Z",
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
            "value": "2023-04-05T21:20:39.8870000Z",
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
        "position": "Entry No.=CONST(871),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 871,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 871,
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
            "value": 871,
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
            "value": "106180",
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
            "value": "LP-01186",
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
            "value": "{ADCDEBB1-F7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T21:20:39.8700000Z",
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
            "value": "2023-04-05T21:20:39.8870000Z",
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
        "position": "Entry No.=CONST(872),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 872,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 872,
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
            "value": 872,
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
            "value": "106180",
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
            "value": "I19",
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
            "value": "LP-01187",
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
            "value": "{2740A1D0-F7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T21:21:33.3970000Z",
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
            "value": "2023-04-05T21:21:33.4100000Z",
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
        "position": "Entry No.=CONST(873),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 873,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 873,
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
            "value": 873,
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
            "value": "106180",
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
            "value": "I20",
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
            "value": "LP-01187",
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
            "value": "{2840A1D0-F7D3-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T21:21:33.3970000Z",
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
            "value": "2023-04-05T21:21:33.4100000Z",
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
        "position": "Entry No.=CONST(877),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 877,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 877,
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
            "value": 877,
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
            "value": "106180",
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
            "value": "I21",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "USER_7686CD7302F5474A8262E2A392556C7A",
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
            "value": "LP-01198",
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
            "value": "{BE868AB5-FDD3-ED11-A7C7-000D3A9205A2}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:03:35.4300000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:54:29.5370000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(878),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 878,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 878,
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
            "value": 878,
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
            "value": "106180",
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
            "value": "I22",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "USER_7686CD7302F5474A8262E2A392556C7A",
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
            "value": "LP-01198",
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
            "value": "{BF868AB5-FDD3-ED11-A7C7-000D3A9205A2}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:03:35.4300000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:54:29.5370000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(879),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 879,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 879,
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
            "value": 879,
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
            "value": "106180",
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
            "value": "I23",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "USER_7686CD7302F5474A8262E2A392556C7A",
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
            "value": "LP-01198",
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
            "value": "{C0868AB5-FDD3-ED11-A7C7-000D3A9205A2}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:03:35.4300000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:54:29.5370000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(882),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 882,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 882,
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
            "value": 882,
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
            "value": "106181",
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
            "value": "I27",
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
            "value": "LP-01192",
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
            "value": "{20125E03-01D4-ED11-A7C7-6045BD372B85}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:27:19.1030000Z",
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
            "value": "2023-04-05T22:27:19.7930000Z",
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
        "position": "Entry No.=CONST(883),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 883,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 883,
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
            "value": 883,
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
            "value": "106181",
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
            "value": "I28",
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
            "value": "LP-01192",
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
            "value": "{21125E03-01D4-ED11-A7C7-6045BD372B85}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:27:19.1030000Z",
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
            "value": "2023-04-05T22:27:19.7930000Z",
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
        "position": "Entry No.=CONST(884),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 884,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 884,
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
            "value": 884,
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
            "value": "106182",
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
            "value": "I33",
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
            "value": "LP-01196",
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
            "value": "{914547F9-01D4-ED11-A7C7-6045BD372B85}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:34:12.4070000Z",
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
            "value": "2023-04-05T22:34:12.4530000Z",
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
        "position": "Entry No.=CONST(885),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 885,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 885,
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
            "value": 885,
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
            "value": "106182",
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
            "value": "I34",
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
            "value": "LP-01196",
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
            "value": "{924547F9-01D4-ED11-A7C7-6045BD372B85}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T22:34:12.4070000Z",
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
            "value": "2023-04-05T22:34:12.4700000Z",
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
        "position": "Entry No.=CONST(916),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 916,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 916,
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
            "value": 916,
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
            "value": "2023-04-10",
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
            "value": "106182",
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
            "value": "I211",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "IVAN.LABRADOR",
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
            "value": "LP-01199",
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
            "value": "{153D853A-07D4-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T23:11:52.9070000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T23:11:57.9370000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(917),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 917,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 917,
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
            "value": 917,
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
            "value": "2023-04-10",
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
            "value": "106182",
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
            "value": "I221",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "IVAN.LABRADOR",
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
            "value": "LP-01199",
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
            "value": "{163D853A-07D4-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T23:11:52.9230000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T23:11:57.9530000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(918),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 918,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 918,
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
            "value": 918,
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
            "value": "2023-04-10",
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
            "value": "106182",
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
            "value": "I231",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "IVAN.LABRADOR",
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
            "value": "LP-01199",
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
            "value": "{173D853A-07D4-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-05T23:11:52.9230000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-05T23:11:57.9530000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(954),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 954,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 954,
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
            "value": 954,
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
            "value": "2023-04-10",
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
            "value": "106185",
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
            "value": 20000,
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
            "value": "I80",
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
            "value": "LP-01231",
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
            "value": "{FB25DF20-EAD7-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-10T21:53:30.2170000Z",
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
            "value": "2023-04-10T21:53:30.3270000Z",
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
        "position": "Entry No.=CONST(955),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 955,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 955,
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
            "value": 955,
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
            "value": "2023-04-10",
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
            "value": "106185",
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
            "value": 20000,
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
            "value": "I81",
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
            "value": "LP-01231",
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
            "value": "{FC25DF20-EAD7-ED11-A7C9-000D3A9FD6E8}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-10T21:53:30.2470000Z",
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
            "value": "2023-04-10T21:53:30.3270000Z",
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
        "position": "Entry No.=CONST(1019),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1019,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1019,
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
            "value": 1019,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-18",
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
            "value": "106189",
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
            "value": 30000,
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
            "value": "I2004",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "USER_7686CD7302F5474A8262E2A392556C7A",
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
            "value": null,
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
            "value": "{FCABD2B6-29DE-ED11-A7C7-00224848B696}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T20:43:47.0630000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-18T20:43:47.0630000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(1020),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1020,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1020,
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
            "value": 1020,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-18",
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
            "value": "106189",
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
            "value": 30000,
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
            "value": "I2005",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "USER_7686CD7302F5474A8262E2A392556C7A",
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
            "value": null,
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
            "value": "{FDABD2B6-29DE-ED11-A7C7-00224848B696}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T20:43:47.0630000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-18T20:43:47.0630000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(1021),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1021,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1021,
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
            "value": 1021,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-18",
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
            "value": "106189",
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
            "value": 30000,
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
            "value": "I2006",
            "System": false
          },
          {
            "id": 25,
            "name": "CreatedBy",
            "type": "Code",
            "value": "USER_7686CD7302F5474A8262E2A392556C7A",
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
            "value": null,
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
            "value": "{FEABD2B6-29DE-ED11-A7C7-00224848B696}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T20:43:47.0800000Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2023-04-18T20:43:47.0800000Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{07B41444-2B13-47B4-9309-43D8A0B0013A}",
            "System": false
          }
        ]
      },
      {
        "id": 337,
        "name": "ReservationEntry",
        "company": "CRONUS USA, Inc.",
        "position": "Entry No.=CONST(1036),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1036,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1036,
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
            "value": 1036,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-18",
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
            "value": "106195",
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
            "value": "I239",
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
            "value": null,
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
            "value": "{6D386F58-3ADE-ED11-A7CA-000D3A9FDE33}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T22:42:51.1030000Z",
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
            "value": "2023-04-18T22:42:51.1030000Z",
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
        "position": "Entry No.=CONST(1037),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1037,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1037,
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
            "value": 1037,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-18",
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
            "value": "106195",
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
            "value": "I240",
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
            "value": null,
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
            "value": "{6E386F58-3ADE-ED11-A7CA-000D3A9FDE33}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T22:42:51.1030000Z",
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
            "value": "2023-04-18T22:42:51.1030000Z",
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
        "position": "Entry No.=CONST(1038),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1038,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1038,
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
            "value": 1038,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-18",
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
            "value": "106195",
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
            "value": "I241",
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
            "value": null,
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
            "value": "{6F386F58-3ADE-ED11-A7CA-000D3A9FDE33}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T22:42:51.1030000Z",
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
            "value": "2023-04-18T22:42:51.1030000Z",
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
        "position": "Entry No.=CONST(1039),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1039,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1039,
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
            "value": 1039,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1004",
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
            "value": 5.0,
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
            "value": "2023-04-18",
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
            "value": "106196",
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
            "value": null,
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
            "value": 5.0,
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
            "value": 5.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 5.0,
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
            "value": "LOT6",
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
            "value": "Lot No.",
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
            "value": null,
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
            "value": "{F8170B9F-3CDE-ED11-A7C7-00224848B696}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T22:59:07.6070000Z",
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
            "value": "2023-04-18T22:59:07.6070000Z",
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
        "position": "Entry No.=CONST(1040),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1040,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1040,
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
            "value": 1040,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1004",
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
            "value": 5.0,
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
            "value": "2023-04-18",
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
            "value": "106196",
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
            "value": null,
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
            "value": 5.0,
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
            "value": 5.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 5.0,
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
            "value": "LOT7",
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
            "value": "Lot No.",
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
            "value": null,
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
            "value": "{F9170B9F-3CDE-ED11-A7C7-00224848B696}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-18T22:59:07.6200000Z",
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
            "value": "2023-04-18T22:59:07.6200000Z",
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
        "position": "Entry No.=CONST(1041),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1041,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1041,
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
            "value": 1041,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 20000,
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
            "value": "I240",
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
            "value": null,
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
            "value": "{C15F4968-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:42:29.3070000Z",
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
            "value": "2023-04-19T14:42:29.3070000Z",
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
        "position": "Entry No.=CONST(1042),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1042,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1042,
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
            "value": 1042,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 20000,
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
            "value": "I241",
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
            "value": null,
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
            "value": "{C25F4968-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:42:29.3400000Z",
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
            "value": "2023-04-19T14:42:29.3400000Z",
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
        "position": "Entry No.=CONST(1043),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1043,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1043,
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
            "value": 1043,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 20000,
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
            "value": "I243",
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
            "value": null,
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
            "value": "{C35F4968-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:42:29.3400000Z",
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
            "value": "2023-04-19T14:42:29.3400000Z",
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
        "position": "Entry No.=CONST(1044),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1044,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1044,
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
            "value": 1044,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1004",
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
            "value": 9.0,
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 30000,
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
            "value": null,
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
            "value": 9.0,
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
            "value": 9.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 9.0,
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
            "value": "LOT10",
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
            "value": "Lot No.",
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
            "value": null,
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
            "value": "{D7952279-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:42:57.5770000Z",
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
            "value": "2023-04-19T14:42:57.5770000Z",
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
        "position": "Entry No.=CONST(1045),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1045,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1045,
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
            "value": 1045,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1004",
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
            "value": 9.0,
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 30000,
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
            "value": null,
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
            "value": 9.0,
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
            "value": 9.0,
            "System": false
          },
          {
            "id": 51,
            "name": "QtytoInvoiceBase",
            "type": "Decimal",
            "value": 9.0,
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
            "value": "LOT11",
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
            "value": "Lot No.",
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
            "value": null,
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
            "value": "{A02286B6-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:44:50.5730000Z",
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
            "value": "2023-04-19T14:44:50.5730000Z",
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
        "position": "Entry No.=CONST(1046),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1046,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1046,
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
            "value": 1046,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 20000,
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
            "value": "I244",
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
            "value": null,
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
            "value": "{512CA4EC-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:46:11.3630000Z",
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
            "value": "2023-04-19T14:46:11.3630000Z",
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
        "position": "Entry No.=CONST(1047),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1047,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1047,
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
            "value": 1047,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 20000,
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
            "value": "I245",
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
            "value": null,
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
            "value": "{522CA4EC-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:46:11.3770000Z",
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
            "value": "2023-04-19T14:46:11.3770000Z",
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
        "position": "Entry No.=CONST(1048),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1048,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1048,
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
            "value": 1048,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-19",
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
            "value": "106197",
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
            "value": 20000,
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
            "value": "I246",
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
            "value": null,
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
            "value": "{532CA4EC-C0DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T14:46:11.3770000Z",
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
            "value": "2023-04-19T14:46:11.3770000Z",
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
        "position": "Entry No.=CONST(1049),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1049,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1049,
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
            "value": 1049,
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
            "value": "2023-04-19",
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
            "value": "106189",
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
            "value": 20000,
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
            "value": "I300",
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
            "value": "LP-01336",
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
            "value": "{93E361F5-E5DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T19:11:17.4070000Z",
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
            "value": "2023-04-19T19:11:17.9370000Z",
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
        "position": "Entry No.=CONST(1050),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1050,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1050,
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
            "value": 1050,
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
            "value": "2023-04-19",
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
            "value": "106189",
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
            "value": 20000,
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
            "value": "I3001",
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
            "value": "LP-01336",
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
            "value": "{94E361F5-E5DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T19:11:17.4370000Z",
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
            "value": "2023-04-19T19:11:17.9370000Z",
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
        "position": "Entry No.=CONST(1051),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1051,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1051,
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
            "value": 1051,
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
            "value": "2023-04-19",
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
            "value": "106189",
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
            "value": 20000,
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
            "value": "I3002",
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
            "value": "LP-01337",
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
            "value": "{316C249F-E6DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T19:16:02.2170000Z",
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
            "value": "2023-04-19T19:16:02.2630000Z",
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
        "position": "Entry No.=CONST(1052),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1052,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1052,
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
            "value": 1052,
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
            "value": "2023-04-19",
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
            "value": "106189",
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
            "value": 20000,
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
            "value": "I3003",
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
            "value": "LP-01337",
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
            "value": "{326C249F-E6DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T19:16:02.2170000Z",
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
            "value": "2023-04-19T19:16:02.2630000Z",
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
        "position": "Entry No.=CONST(1053),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1053,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1053,
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
            "value": 1053,
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
            "value": "2023-04-19",
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
            "value": "106189",
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
            "value": 20000,
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
            "value": "I3005",
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
            "value": "LP-01338",
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
            "value": "{E1B1C979-E7DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T19:22:09.0430000Z",
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
            "value": "2023-04-19T19:22:09.1070000Z",
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
        "position": "Entry No.=CONST(1054),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1054,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1054,
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
            "value": 1054,
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
            "value": "2023-04-19",
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
            "value": "106189",
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
            "value": 20000,
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
            "value": "I3006",
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
            "value": "LP-01338",
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
            "value": "{E2B1C979-E7DE-ED11-A7C7-00224844980C}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-19T19:22:09.0430000Z",
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
            "value": "2023-04-19T19:22:09.1370000Z",
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
        "position": "Entry No.=CONST(1087),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1087,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1087,
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
            "value": 1087,
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
            "value": "2023-04-20",
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
            "value": "106200",
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
            "value": 20000,
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
            "value": "I3033",
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
            "value": "LP-01403",
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
            "value": "{00418F60-95DF-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-20T16:07:03.2570000Z",
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
            "value": "2023-04-20T16:07:03.3200000Z",
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
        "position": "Entry No.=CONST(1088),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1088,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1088,
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
            "value": 1088,
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
            "value": "2023-04-20",
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
            "value": "106200",
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
            "value": 20000,
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
            "value": "I3034",
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
            "value": "LP-01403",
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
            "value": "{01418F60-95DF-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-20T16:07:03.2730000Z",
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
            "value": "2023-04-20T16:07:03.3200000Z",
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
        "position": "Entry No.=CONST(1089),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1089,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1089,
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
            "value": 1089,
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
            "value": "2023-04-20",
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
            "value": "106201",
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
            "value": 20000,
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
            "value": "I3035",
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
            "value": "LP-01407",
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
            "value": "{ED5A86C4-95DF-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-20T16:09:53.4270000Z",
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
            "value": "2023-04-20T16:09:53.4730000Z",
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
        "position": "Entry No.=CONST(1090),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1090,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1090,
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
            "value": 1090,
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
            "value": "2023-04-20",
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
            "value": "106201",
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
            "value": 20000,
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
            "value": "I3036",
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
            "value": "LP-01407",
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
            "value": "{EE5A86C4-95DF-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-20T16:09:53.4430000Z",
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
            "value": "2023-04-20T16:09:53.4900000Z",
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
        "position": "Entry No.=CONST(1109),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1109,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1109,
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
            "value": 1109,
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
            "value": "2023-04-21",
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
            "value": "106194",
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
            "value": 20000,
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
            "value": "I4000",
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
            "value": "LP-01437",
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
            "value": "{4619B19E-53E0-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-21T14:48:51.1430000Z",
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
            "value": "2023-04-21T14:48:51.2670000Z",
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
        "position": "Entry No.=CONST(1110),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1110,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1110,
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
            "value": 1110,
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
            "value": "2023-04-21",
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
            "value": "106194",
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
            "value": 20000,
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
            "value": "I4001",
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
            "value": "LP-01437",
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
            "value": "{4719B19E-53E0-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-21T14:48:51.1730000Z",
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
            "value": "2023-04-21T14:48:51.2830000Z",
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
        "position": "Entry No.=CONST(1117),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1117,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1117,
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
            "value": 1117,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-21",
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
            "value": "106206",
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
            "value": "I4003",
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
            "value": null,
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
            "value": "{1712E1A1-64E0-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-21T16:50:34.5570000Z",
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
            "value": "2023-04-21T16:50:34.5570000Z",
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
        "position": "Entry No.=CONST(1118),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1118,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1118,
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
            "value": 1118,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-04-21",
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
            "value": "106206",
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
            "value": "I4004",
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
            "value": null,
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
            "value": "{1812E1A1-64E0-ED11-A7C9-000D3A9FDEE1}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-21T16:50:34.5570000Z",
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
            "value": "2023-04-21T16:50:34.5570000Z",
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
        "position": "Entry No.=CONST(1119),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1119,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1119,
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
            "value": 1119,
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
            "value": "2023-04-25",
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
            "value": "106209",
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
            "value": 20000,
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
            "value": "J11",
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
            "value": "LP-01449",
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
            "value": "{6E8F77B9-ABE3-ED11-8848-6045BD349105}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-25T20:57:09.2130000Z",
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
            "value": "2023-04-25T20:57:09.3230000Z",
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
        "position": "Entry No.=CONST(1120),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1120,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1120,
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
            "value": 1120,
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
            "value": "2023-04-25",
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
            "value": "106209",
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
            "value": 20000,
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
            "value": "J12",
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
            "value": "LP-01449",
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
            "value": "{6F8F77B9-ABE3-ED11-8848-6045BD349105}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-25T20:57:09.2270000Z",
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
            "value": "2023-04-25T20:57:09.3370000Z",
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
        "position": "Entry No.=CONST(1121),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1121,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1121,
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
            "value": 1121,
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
            "value": "2023-04-25",
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
            "value": "106209",
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
            "value": 20000,
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
            "value": "J13",
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
            "value": "LP-01450",
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
            "value": "{0BEEF9CC-ABE3-ED11-8848-6045BD349105}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-25T20:57:44.2900000Z",
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
            "value": "2023-04-25T20:57:44.3230000Z",
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
        "position": "Entry No.=CONST(1122),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1122,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1122,
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
            "value": 1122,
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
            "value": "2023-04-25",
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
            "value": "106209",
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
            "value": 20000,
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
            "value": "J14",
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
            "value": "LP-01450",
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
            "value": "{0CEEF9CC-ABE3-ED11-8848-6045BD349105}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-04-25T20:57:44.2900000Z",
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
            "value": "2023-04-25T20:57:44.3370000Z",
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
        "position": "Entry No.=CONST(1154),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1154,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1154,
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
            "value": 1154,
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
            "value": "2023-05-10",
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
            "value": "106215",
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
            "value": 30000,
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
            "value": "WW",
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
            "value": "LP-01482",
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
            "value": "{EED5F982-50EF-ED11-8848-000D3AA548C6}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-05-10T16:34:27.5070000Z",
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
            "value": "2023-05-10T16:34:28.1030000Z",
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
        "position": "Entry No.=CONST(1155),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1155,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1155,
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
            "value": 1155,
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
            "value": "2023-05-10",
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
            "value": "106215",
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
            "value": 30000,
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
            "value": "WWWW",
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
            "value": "LP-01482",
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
            "value": "{EFD5F982-50EF-ED11-8848-000D3AA548C6}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-05-10T16:34:27.5330000Z",
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
            "value": "2023-05-10T16:34:28.1100000Z",
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
        "position": "Entry No.=CONST(1156),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1156,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1156,
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
            "value": 1156,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-05-10",
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
            "value": "106215",
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
            "value": 20000,
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
            "value": "1111A",
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
            "value": null,
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
            "value": "{F5B0FD46-53EF-ED11-8848-000D3AA548C6}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-05-10T16:54:09.0870000Z",
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
            "value": "2023-05-10T16:54:09.0870000Z",
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
        "position": "Entry No.=CONST(1157),Positive=CONST(Yes)",
        "recordId": "Reservation Entry: 1157,Yes",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "EntryNo",
              "type": "Integer",
              "value": 1157,
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
            "value": 1157,
            "System": false
          },
          {
            "id": 2,
            "name": "ItemNo",
            "type": "Code",
            "value": "1005",
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
            "value": "2023-05-10",
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
            "value": "106215",
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
            "value": 20000,
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
            "value": "1111B",
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
            "value": null,
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
            "value": "{F6B0FD46-53EF-ED11-8848-000D3AA548C6}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2023-05-10T16:54:09.1000000Z",
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
            "value": "2023-05-10T16:54:09.1000000Z",
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
    "Error": "The TrackingSpecification for NEWWMS does not exist."
  },
  "ItemTrackingJO": {}
}`
