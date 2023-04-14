
**Input:**

```
{
  "ProcessMethod": "Assign_ItemChild_to_LP_Pallet_From_WR_With_SNLOT",
  "Parameters": [
    {
      "WarhouseReceiptNo": "WHSE REC-00159",
      "BinCode": "REC-1",
      "Item_Child": [
        {
          "ItemNo": "1013",
          "TotalToReceive": 3,
          "UnitofMeasureCode": "PCS",
          "SourceNo": "106180",
          "SourceRefNo": 10000,
          "LineNo": 10000,
          "TrackingInfo": [
            {
              "LotNo": "",
              "SerialNo": "I211",
              "ExperationDate": "",
              "Qty": 1
            },
            {
              "LotNo": "",
              "SerialNo": "I221",
              "ExperationDate": "",
              "Qty": 1
            },
            {
              "LotNo": "",
              "SerialNo": "I231",
              "ExperationDate": "",
              "Qty": 1
            }
          ]
        },
        {
          "Item_Child_No": "1013",
          "TotalToReceive": 3,
          "UnitofMeasureCode": "PCS",
          "SourceNo": "106180",
          "SourceRefNo": 10000,
          "LineNo": 10000,
          "TrackingInfo": [
            {
              "LotNo": "",
              "SerialNo": "I211",
              "ExperationDate": "",
              "Qty": 1
            },
            {
              "LotNo": "",
              "SerialNo": "I221",
              "ExperationDate": "",
              "Qty": 1
            },
            {
              "LotNo": "",
              "SerialNo": "I231",
              "ExperationDate": "",
              "Qty": 1
            }
          ]
        }
      ]
    }
  ]
}
```

Ouput:

```
{
  "TrackingSpecificationOpen": [
    {
      "id": 337,
      "name": "ReservationEntry",
      "company": "CRONUS USA, Inc.",
      "position": "Entry No.=CONST(11),Positive=CONST(Yes)",
      "recordId": "Reservation Entry: 11,Yes",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 11,
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
          "value": 11,
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
          "value": "2022-12-22",
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
          "value": "106013",
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
          "value": "SERIAL20000",
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
          "value": "2022-12-22",
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
          "value": "LOT20000",
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
          "value": "Lot and Serial No.",
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
          "value": "{50570DEE-3C82-ED11-9989-6045BDF7747D}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-12-22T21:09:33.2000000Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{F488FB98-1985-40BE-8E78-F686150F69E0}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-12-22T21:09:33.2000000Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{F488FB98-1985-40BE-8E78-F686150F69E0}",
          "System": false
        }
      ]
    },
    {
      "id": 337,
      "name": "ReservationEntry",
      "company": "CRONUS USA, Inc.",
      "position": "Entry No.=CONST(12),Positive=CONST(Yes)",
      "recordId": "Reservation Entry: 12,Yes",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "EntryNo",
            "type": "Integer",
            "value": 12,
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
          "value": 12,
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
          "value": "2022-12-22",
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
          "value": "106013",
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
          "value": "SERIAL20001",
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
          "value": "2022-12-22",
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
          "value": "LOT20000",
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
          "value": "Lot and Serial No.",
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
          "value": "{9E07D510-3D82-ED11-9989-6045BDF7747D}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-12-22T21:10:31.5370000Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{F488FB98-1985-40BE-8E78-F686150F69E0}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-12-22T21:10:31.5370000Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{F488FB98-1985-40BE-8E78-F686150F69E0}",
          "System": false
        }
      ]
    }
  ]
}
```

**Result in Busines Central:**

![image.png](/.attachments/image-94f33d7d-ad6c-4251-8164-76e85b630125.png)

