**Input**

```
{
  "ProcessMethod": "GetItemTrackingSpecification",
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
  "TrackingSpecification": [
    {
      "id": 337,
      "name": "ReservationEntry",
      "company": "CRONUS USA, Inc.",
      "position": "Entry No.=CONST(4),Positive=CONST(Yes)",
      "recordId": "Reservation Entry: 4,Yes",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 4,
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
      "fieldCount": 50,
      "fields": [
        {
          "id": 1,
          "name": "EntryNo",
          "type": "Integer",
          "value": 4,
          "System": false
        },
        {
          "id": 2,
          "name": "ItemNo",
          "type": "Code",
          "value": "1000",
          "System": false
        },
        {
          "id": 3,
          "name": "LocationCode",
          "type": "Code",
          "value": "WMS",
          "System": false
        },
        {
          "id": 4,
          "name": "Quantity(Base)",
          "type": "Decimal",
          "value": 10.0,
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
          "value": "2022-11-30",
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
          "value": "106014",
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
          "value": "2022-12-01",
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
          "value": 10.0,
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
          "name": "QtytoHandle(Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 51,
          "name": "QtytoInvoice(Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 53,
          "name": "QuantityInvoiced(Base)",
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
          "value": "LOT0006",
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
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{1BA269CD-9780-ED11-9989-6045BDF778D8}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-12-20T18:55:06.6070000Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{8C306CEC-9612-4222-9B2D-738FAC873B57}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-12-20T18:55:06.6070000Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{8C306CEC-9612-4222-9B2D-738FAC873B57}",
          "System": false
        }
      ]
    }
  ]
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
