**Request:**

```
{
  "ProcessMethod": "GetQtyPhysInventoryByItemNo",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "ItemNo": "10110",
      "VariantCode": "VN40-9",
      "LineNo": 450000
    }
  ]
}
```

**Output:**
```
{
  "QtyPhysInventoryByItemNo": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "BinCode": "",
      "LineNo": 450000,
      "LocationCode": "MAUI-RET",
      "ItemNo": "10110",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 2.0,
      "QtyPhysInventory": 4.0,
      "VariantCode": "VN40-9",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    }
  ],
  "Duration": "13 milliseconds"
}
```


