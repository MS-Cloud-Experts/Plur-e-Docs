**ProcessMethod**: Get_WarehouseInvPhysicalCount

**Description**:
This method returns an array of Warehouse Journals Lines special to the physical count given a Location.

**Input**:
**Parameters**: 
-	**LocationCode**: Specific Location where you want to perform the inventory count.

**Ouput**: 
-The process will be executed correctly if it returns the lines of the Warehouse Item Journal.
-	**Warehouse_Physical_Inventory_Journal**: Array of Warehouse Journals Lines.

**Example**:

Request:

`jsonRequest":"{\"ProcessMethod\":\"Get_WarehouseInvPhysicalCount\",\"Parameters\":[{\"LocationCode\":\"CCC\"}]}`

**Outputs**:


```
{
  "Warehouse_Physical_Inventory_Journal": [
    {
      "id": 7311,
      "name": "WarehouseJournalLine",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(10000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,10000",
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
            "value": "CCC",
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
          "value": "PLUR-E",
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
          "value": "CCC",
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
          "value": "PARIS Guest Chair, black",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1900-S",
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
          "value": "T00016",
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
          "value": "LP000442",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3AFA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.047Z",
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
          "value": "2022-04-20T14:46:38.047Z",
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
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(20000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,20000",
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
            "value": "CCC",
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
          "value": "PLUR-E",
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
          "value": "CCC",
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
          "value": "PARIS Guest Chair, black",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1900-S",
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
          "value": "T00016",
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
          "value": "LP000443",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3BFA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.047Z",
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
          "value": "2022-04-20T14:46:38.047Z",
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
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(30000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,30000",
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
            "value": "CCC",
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
          "value": "PLUR-E",
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
          "value": "CCC",
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
          "value": "PARIS Guest Chair, black",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1900-S",
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
          "value": "T00016",
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
          "value": "LP000444",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3CFA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.047Z",
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
          "value": "2022-04-20T14:46:38.047Z",
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
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(40000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,40000",
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
            "value": "CCC",
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
          "value": "CCC",
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
          "value": "PARIS Guest Chair, black",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1900-S",
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
          "value": "T00016",
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
          "value": "LP000445",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3DFA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.047Z",
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
          "value": "2022-04-20T14:46:38.047Z",
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
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(50000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,50000",
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
            "value": "CCC",
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
          "value": "CCC",
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
          "value": "MOSCOW Swivel Chair, red",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1980-S",
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
          "value": "T00016",
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
          "value": "LP000477",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3EFA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.077Z",
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
          "value": "2022-04-20T14:46:38.077Z",
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
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(60000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,60000",
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
            "value": "CCC",
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
          "value": "PLUR-E",
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
          "value": "CCC",
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
          "value": "MOSCOW Swivel Chair, red",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1980-S",
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
          "value": "T00016",
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
          "value": "LP000478",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{3FFA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.077Z",
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
          "value": "2022-04-20T14:46:38.077Z",
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
      "position": "Journal Template Name=CONST(PHYSICAL I),Journal Batch Name=CONST(PLUR-E),Location Code=CONST(CCC),Line No.=CONST(80000)",
      "recordId": "Warehouse Journal Line: PHYSICAL I,PLUR-E,CCC,80000",
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
            "value": "CCC",
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
          "value": "PLUR-E",
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
          "value": "CCC",
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
          "value": "PARIS Guest Chair, black",
          "System": false
        },
        {
          "id": 9,
          "name": "ItemNo",
          "type": "Code",
          "value": "1900-S",
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
          "value": "T00016",
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
          "value": "LP000441",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{41FA2EAE-B8C0-EC11-8AA5-002248A68B4E}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-04-20T14:46:38.11Z",
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
          "value": "2022-04-20T14:46:38.11Z",
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

**Errors**:
```
{
  "Error": {
    "Code": "Not found",
    "Message": "The Location Code (CCCa) was not found"
  }
}
```


