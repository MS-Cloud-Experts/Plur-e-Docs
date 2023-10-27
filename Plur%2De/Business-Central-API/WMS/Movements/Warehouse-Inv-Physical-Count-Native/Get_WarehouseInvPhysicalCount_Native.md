**Request:**

```
{
  "ProcessMethod": "Get_WarehouseInvPhysicalCount_Native",
  "Parameters": [
    {
      "Journal Template Name": "PHYSICAL I",
      "Journal Batch Name": "DEFAULT"
    }
  ]
}
```

**Ouput:**
```
[
  {
    "JournalTemplateName": "PHYSICAL I",
    "JournalBatchName": "DEFAULT",
    "LineNo": 30000,
    "RegisteringDate": "2023-04-10",
    "LocationCode": "LOC_TEST",
    "ItemNo": "1896-S",
    "Qty(PhysInventory)": 4.0,
    "UserID": "IVAN.LABRADOR",
    "VariantCode": "",
    "SerialNo": "",
    "LotNo": ""
  },
  {
    "JournalTemplateName": "PHYSICAL I",
    "JournalBatchName": "DEFAULT",
    "LineNo": 40000,
    "RegisteringDate": "2023-04-10",
    "LocationCode": "LOC_TEST",
    "ItemNo": "1900-S",
    "Qty(PhysInventory)": 998.0,
    "UserID": "IVAN.LABRADOR",
    "VariantCode": "",
    "SerialNo": "",
    "LotNo": ""
  },
  {
    "JournalTemplateName": "PHYSICAL I",
    "JournalBatchName": "DEFAULT",
    "LineNo": 50000,
    "RegisteringDate": "2023-04-10",
    "LocationCode": "LOC_TEST",
    "ItemNo": "1896-S",
    "Qty(PhysInventory)": 996.0,
    "UserID": "IVAN.LABRADOR",
    "VariantCode": "",
    "SerialNo": "",
    "LotNo": ""
  }
]
```

