**Input**

```
{
  "ProcessMethod": "GetItemTracking",
  "Parameters": [
    {
      "Code": "FREEENTRY"
    }
  ]
}
```


**OutPut**

```
{
  "ItemTracking": {
    "id": 6502,
    "name": "ItemTrackingCode",
    "company": "CRONUS USA, Inc.",
    "position": "Code=CONST(FREEENTRY)",
    "recordId": "Item Tracking Code: FREEENTRY",
    "primaryKey": {
      "fieldCount": 1,
      "fields": [
        {
          "id": 1,
          "name": "Code",
          "type": "Code",
          "value": "FREEENTRY",
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
        "value": "FREEENTRY",
        "System": false
      },
      {
        "id": 2,
        "name": "Description",
        "type": "Text",
        "value": "Free entry of tracking",
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
        "value": true,
        "System": false
      },
      {
        "id": 11,
        "name": "SNSpecificTracking",
        "type": "Boolean",
        "value": false,
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
        "value": false,
        "System": false
      },
      {
        "id": 21,
        "name": "SNPurchaseInboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 22,
        "name": "SNPurchaseOutboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 23,
        "name": "SNSalesInboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 24,
        "name": "SNSalesOutboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 25,
        "name": "SNPosAdjmtInbTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 26,
        "name": "SNPosAdjmtOutbTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 27,
        "name": "SNNegAdjmtInbTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 28,
        "name": "SNNegAdjmtOutbTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 29,
        "name": "SNTransferTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 30,
        "name": "SNManufInboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 31,
        "name": "SNManufOutboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 32,
        "name": "SNAssemblyInboundTracking",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 33,
        "name": "SNAssemblyOutboundTracking",
        "type": "Boolean",
        "value": false,
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
        "value": "{E9582523-DF3A-ED11-BBAE-6045BD8E554A}",
        "System": false
      },
      {
        "id": 2000000001,
        "name": "SystemCreatedAt",
        "type": "DateTime",
        "value": "2022-09-23T01:29:20.0130000Z",
        "System": false
      },
      {
        "id": 2000000002,
        "name": "SystemCreatedBy",
        "type": "GUID",
        "value": "{00000000-0000-0000-0000-000000000001}",
        "System": false
      },
      {
        "id": 2000000003,
        "name": "SystemModifiedAt",
        "type": "DateTime",
        "value": "2022-09-23T01:29:51.4930000Z",
        "System": false
      },
      {
        "id": 2000000004,
        "name": "SystemModifiedBy",
        "type": "GUID",
        "value": "{00000000-0000-0000-0000-000000000001}",
        "System": false
      }
    ]
  }
}
```



**Errors**