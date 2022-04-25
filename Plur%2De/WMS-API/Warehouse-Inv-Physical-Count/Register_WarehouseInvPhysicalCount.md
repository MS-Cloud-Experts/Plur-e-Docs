**ProcessMethod**: PreRegister_WarehouseInvPhysicalCount

**Description**:
This method allows registering a Batch of physical inventory count, generating in turn the update of the Warehouse Entry and the associated License Plates.

**Input**:
**Parameters**: 
-	**JournalTemplateName**: JournalTemplateName.
-	**LocationCode**: Specific Location where you want to perform the inventory count.

**Example**:

Request:

`
"jsonRequest":
{
  "ProcessMethod": "Register_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "LocationCode": "BBB"
    }
  ]
}
`

**Output**: 
-	**Warehouse_Physical_Inventory_Counted**: It contains an array with the lines of the current batch but the lines that have zero quantities have been eliminated.
-	**Warehouse_Physical_Inventory_NoCounted**: It contains an array with the lines of a new Batch, with the lines of the main batch that were counted at Zero.

```
{
  "Warehouse_Physical_Inventory_Counted": [
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(BBB),Line No.=CONST(40000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,BBB,40000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "PLUR-E",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 40000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "PLUR-E",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 40000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ROME Guest Chair, green",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1960-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Positive Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000504",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{9E9CAE8F-B4C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:27:13.647Z",
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
          "value": "2022-04-25T16:27:17.26Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(BBB),Line No.=CONST(50000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,BBB,50000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "PLUR-E",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 50000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "PLUR-E",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 50000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ROME Guest Chair, green",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1960-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Positive Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000505",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{9F9CAE8F-B4C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:27:13.68Z",
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
          "value": "2022-04-25T16:27:17.26Z",
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
  ],
  "Warehouse_Physical_Inventory_NoCounted": [
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(10000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,10000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 10000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 10000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "DAMAGE",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "100A",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "100A",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -5.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -5.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "DAMAGE",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "QUARENTINE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{2C1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.21Z",
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
          "value": "2022-04-25T16:22:01.21Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(20000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,20000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 20000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 20000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "TEST",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "100",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -10.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -10.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{2D1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.21Z",
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
          "value": "2022-04-25T16:22:01.21Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(30000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,30000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 30000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 30000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "100A",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "100A",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -1.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -1.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{2E1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.227Z",
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
          "value": "2022-04-25T16:22:01.227Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(60000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,60000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 60000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 60000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "SEOUL Guest Chair, red",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1988-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -155.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -155.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 155.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 155.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO1",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 155.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 155.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000473",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{2F1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.227Z",
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
          "value": "2022-04-25T16:22:01.227Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(70000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,70000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 70000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 70000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "TEST",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "100",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -10.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -10.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 10.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{301F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.227Z",
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
          "value": "2022-04-25T16:22:01.227Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(80000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,80000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 80000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 80000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "HASSELT, Conference Chair.",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1006",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -40.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -40.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 40.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 40.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 40.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 40.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{311F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.24Z",
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
          "value": "2022-04-25T16:22:01.24Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(90000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,90000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 90000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 90000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "100A",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "100A",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -744.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -744.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 744.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 744.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 744.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 744.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{321F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.24Z",
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
          "value": "2022-04-25T16:22:01.24Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(100000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,100000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 100000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 100000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "MUNICH Swivel Chair, yellow",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1972-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -12.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -12.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 12.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 12.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 12.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 12.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{331F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.257Z",
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
          "value": "2022-04-25T16:22:01.257Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(110000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,110000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 110000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 110000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "SEOUL Guest Chair, red",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1988-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -4.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -4.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 4.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 4.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 4.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 4.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000474",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{341F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.257Z",
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
          "value": "2022-04-25T16:22:01.257Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(120000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,120000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 120000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 120000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "SEOUL Guest Chair, red",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1988-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000475",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{351F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.257Z",
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
          "value": "2022-04-25T16:22:01.257Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(130000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,130000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 130000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 130000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "SEOUL Guest Chair, red",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1988-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000476",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{361F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.257Z",
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
          "value": "2022-04-25T16:22:01.257Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(140000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,140000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 140000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 140000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000465",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{371F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.257Z",
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
          "value": "2022-04-25T16:22:01.257Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(150000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,150000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 150000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 150000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -1.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -1.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000466",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{381F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.273Z",
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
          "value": "2022-04-25T16:22:01.273Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(160000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,160000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 160000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 160000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -1.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -1.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000467",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{391F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.273Z",
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
          "value": "2022-04-25T16:22:01.273Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(170000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,170000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 170000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 170000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000468",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3A1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.273Z",
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
          "value": "2022-04-25T16:22:01.273Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(180000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,180000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 180000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 180000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000469",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3B1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.273Z",
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
          "value": "2022-04-25T16:22:01.273Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(190000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,190000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 190000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 190000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000470",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3C1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.273Z",
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
          "value": "2022-04-25T16:22:01.273Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(200000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,200000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 200000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 200000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000471",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3D1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.287Z",
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
          "value": "2022-04-25T16:22:01.287Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(210000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,210000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 210000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 210000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -2.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 2.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000472",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3E1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.287Z",
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
          "value": "2022-04-25T16:22:01.287Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(220000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,220000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 220000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 220000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "ATLANTA Whiteboard, base",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1996-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -5.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -5.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 5.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000514",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3F1F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.287Z",
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
          "value": "2022-04-25T16:22:01.287Z",
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
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(NON COUNT),Location Code=CONST(BBB),Line No.=CONST(230000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,NON COUNT,BBB,230000",
      "primaryKey": {
        "fieldCount": 4,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "JournalBatchName",
            "type": "Code",
            "value": "NON COUNT",
            "System": false
          },
          {
            "id": 5,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": false
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 230000,
            "System": false
          }
        ]
      },
      "fieldCount": 63,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "JournalBatchName",
          "type": "Code",
          "value": "NON COUNT",
          "System": false
        },
        {
          "id": 3,
          "name": "LineNo",
          "type": "Integer",
          "value": 230000,
          "System": false
        },
        {
          "id": 4,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-04-19",
          "System": false
        },
        {
          "id": 5,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 6,
          "name": "FromZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 7,
          "name": "FromBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 8,
          "name": "Description",
          "type": "Text",
          "value": "SYDNEY Swivel Chair, green",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "2000-S",
          "System": false
        },
        {
          "id": 10,
          "name": "Quantity",
          "type": "Decimal",
          "value": -77.0,
          "System": false
        },
        {
          "id": 11,
          "name": "Qty(Base)",
          "type": "Decimal",
          "value": -77.0,
          "System": false
        },
        {
          "id": 12,
          "name": "Qty(Absolute)",
          "type": "Decimal",
          "value": 77.0,
          "System": false
        },
        {
          "id": 13,
          "name": "Qty(Absolute,Base)",
          "type": "Decimal",
          "value": 77.0,
          "System": false
        },
        {
          "id": 14,
          "name": "ZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 15,
          "name": "BinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 20,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 21,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 22,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 23,
          "name": "SourceLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 24,
          "name": "SourceSublineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 25,
          "name": "SourceDocument",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 26,
          "name": "SourceCode",
          "type": "Code",
          "value": "WHPHYSINVT",
          "System": false
        },
        {
          "id": 27,
          "name": "ToZoneCode",
          "type": "Code",
          "value": "STO",
          "System": false
        },
        {
          "id": 28,
          "name": "ToBinCode",
          "type": "Code",
          "value": "AJUST",
          "System": false
        },
        {
          "id": 29,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 33,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 35,
          "name": "FromBinTypeCode",
          "type": "Code",
          "value": "STORAGE",
          "System": false
        },
        {
          "id": 40,
          "name": "Cubage",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 41,
          "name": "Weight",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 50,
          "name": "WhseDocumentNo",
          "type": "Code",
          "value": "T00021",
          "System": false
        },
        {
          "id": 51,
          "name": "WhseDocumentType",
          "type": "Option",
          "value": "Whse. Phys. Inventory",
          "System": false
        },
        {
          "id": 52,
          "name": "WhseDocumentLineNo",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 53,
          "name": "Qty(Calculated)",
          "type": "Decimal",
          "value": 77.0,
          "System": false
        },
        {
          "id": 54,
          "name": "Qty(PhysInventory)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 55,
          "name": "EntryType",
          "type": "Option",
          "value": "Negative Adjmt.",
          "System": false
        },
        {
          "id": 56,
          "name": "PhysInventory",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 60,
          "name": "ReferenceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 61,
          "name": "ReferenceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 67,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 68,
          "name": "Qty(Calculated)(Base)",
          "type": "Decimal",
          "value": 77.0,
          "System": false
        },
        {
          "id": 69,
          "name": "Qty(PhysInventory)(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5402,
          "name": "VariantCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5404,
          "name": "QtyperUnitofMeasure",
          "type": "Decimal",
          "value": 1.0,
          "System": false
        },
        {
          "id": 5407,
          "name": "UnitofMeasureCode",
          "type": "Code",
          "value": "PCS",
          "System": false
        },
        {
          "id": 5408,
          "name": "QtyRoundingPrecision",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 5409,
          "name": "QtyRoundingPrecision(Base)",
          "type": "Decimal",
          "value": null,
          "System": false
        },
        {
          "id": 6500,
          "name": "SerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6501,
          "name": "LotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6502,
          "name": "WarrantyDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6503,
          "name": "ExpirationDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6504,
          "name": "NewSerialNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6505,
          "name": "NewLotNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6506,
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
          "id": 7380,
          "name": "PhysInvtCountingPeriodCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7381,
          "name": "PhysInvtCountingPeriodType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLULicensePlates",
          "type": "Code",
          "value": "LP000205",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{401F85D5-B3C4-EC11-8E7E-002248A6810F}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-25T16:22:01.287Z",
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
          "value": "2022-04-25T16:22:01.287Z",
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
```

**Licenses Plate Ledger Entries:**
![image.png](/.attachments/image-59b91d75-849a-4de7-9268-1e2224720718.png)

**Bin Contents:**

![image.png](/.attachments/image-3b2fdb8d-771c-49ff-975e-aac713eb80f5.png)


**Errors:**

`
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The WhseJnlLine was not found in JournalTemplateName=PHYSICAL I and JournalBatchName=PLUR-E."
  }
}
`



