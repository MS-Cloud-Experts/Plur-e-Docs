**Request**
```
{
  "ProcessMethod": "WriteInventoryCountV2",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-13",
      "EntryType": "Positive Adjmt.",
      "DocumentNo": "T00203",
      "ItemNo": "10110",
      "VariantCode": "VN40-9",
      "Description": "L BLACK",
      "LocationCode": "ASIA",
      "SalespersPurchCode": "",
      "QtyCalculated": 2,
      "QtyPhysInventory": 1,
      "Quantity": 0,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "LineNo": 260000,
      "SerialJA": [
        [
          {
            "ItemNo": "SERIAL2",
            "VariantCode": "",
            "LotNo": "",
            "SerialNo": "X14"
          }
        ]
      ]
    },
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-13",
      "EntryType": "Positive Adjmt.",
      "DocumentNo": "T00203",
      "ItemNo": "10110",
      "VariantCode": "4827.9",
      "Description": "L BLACK",
      "LocationCode": "ASIA",
      "SalespersPurchCode": "",
      "QtyCalculated": 2,
      "QtyPhysInventory": 2,
      "Quantity": 0,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "LineNo": 210000
    }
  ]
}

```

**Output:**

```
{
  "WriteInventoryCountV2": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "BinCode": "",
      "LineNo": 320000,
      "LocationCode": "FTLDL-RET",
      "ItemNo": "10110",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 2.0,
      "QtyPhysInventory": 2.0,
      "VariantCode": "4827.9",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    },
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "BinCode": "",
      "LineNo": 450000,
      "LocationCode": "MAUI-RET",
      "ItemNo": "10110",
      "UnitofMeasureCode": "EA",
      "QtyCalculated": 2.0,
      "QtyPhysInventory": 1.0,
      "VariantCode": "VN40-9",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    }
  ],
  "Duration": "4 seconds 17 milliseconds"
}
```

