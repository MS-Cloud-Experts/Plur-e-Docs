**Request:**

```
{
  "ProcessMethod": "Get_InvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT"
    }
  ]
}
```

**Output:**

```
{
  "PhysicalInventoryCount": [
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT",
      "BinCode": "STORAGE",
      "LineNo": 10000,
      "LocationCode": "ASIA",
      "ItemNo": "D1KHAVIH",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 58.0,
      "QtyPhysInventory": 38.0,
      "VariantCode": "BLA00L",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    },
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT",
      "BinCode": "STORAGE",
      "LineNo": 20000,
      "LocationCode": "ASIA",
      "ItemNo": "D1KHAVIH",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 26.0,
      "QtyPhysInventory": 26.0,
      "VariantCode": "BLA00M",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    },
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT",
      "BinCode": "STORAGE",
      "LineNo": 30000,
      "LocationCode": "ASIA",
      "ItemNo": "D1KHAVIH",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 62.0,
      "QtyPhysInventory": 62.0,
      "VariantCode": "BLA00S",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    },
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT",
      "BinCode": "STORAGE",
      "LineNo": 40000,
      "LocationCode": "ASIA",
      "ItemNo": "D1KHAVIH",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 9.0,
      "QtyPhysInventory": 9.0,
      "VariantCode": "BLA0XS",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    }
  ],
  "Duration": "54 milliseconds"
}
```
