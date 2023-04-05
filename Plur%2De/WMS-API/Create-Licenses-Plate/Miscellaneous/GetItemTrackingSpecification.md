**Item Tracking Lines Open:**

![image.png](/.attachments/image-723d75d5-d765-4c0c-8e3c-f6362c9721ff.png)

**Item Tracking:**

![image.png](/.attachments/image-5918d26f-6798-47ce-ab89-1fa604a2f02a.png)

![image.png](/.attachments/image-45d7e8d5-1bc4-4bf7-9b3a-571922e61f0b.png)

**Input**

```
{
  "ProcessMethod": "GetItemTrackingSpecificationOpen",
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
  "TrackingSpecificationOpen": [
    {
      "id": 336,
      "name": "TrackingSpecification",
      "company": "CRONUS USA, Inc.",
      "position": "Entry No.=CONST(663)",
      "recordId": "Tracking Specification: 663",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 663,
            "System": false
          }
        ]
      },
      "fieldCount": 51,
      "fields": [
        {
          "id": 1,
          "name": "EntryNo",
          "type": "Integer",
          "value": 663,
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
          "value": 663,
          "System": false
        },
        {
          "id": 17,
          "name": "TransferItemEntryNo",
          "type": "Integer",
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
          "id": 31,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
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
          "value": "2022-12-20",
          "System": false
        },
        {
          "id": 50,
          "name": "QtytoHandle(Base)",
          "type": "Decimal",
          "value": null,
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
          "id": 52,
          "name": "QuantityHandled(Base)",
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
          "id": 60,
          "name": "QtytoHandle",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 61,
          "name": "QtytoInvoice",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 70,
          "name": "BufferStatus",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71,
          "name": "BufferStatus2",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 72,
          "name": "BufferValue1",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 73,
          "name": "BufferValue2",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 74,
          "name": "BufferValue3",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 75,
          "name": "BufferValue4",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 76,
          "name": "BufferValue5",
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
          "name": "ProhibitCancellation",
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
          "id": 5402,
          "name": "BinCode",
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
          "id": 7300,
          "name": "QuantityactualHandled(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{69C2F8C5-A780-ED11-9989-6045BDF77834}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-12-20T20:49:22.8930000Z",
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
          "value": "2022-12-20T20:49:22.8930000Z",
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
