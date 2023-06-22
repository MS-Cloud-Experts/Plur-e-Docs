**Request:**
```
{
  "ProcessMethod": "Get_ItemReclassJournal",
  "Parameters": [
    {
      "Journal Template Name": "TRANSFER",
      "Journal Batch Name": "DEFAULT"
    }
  ]
}
```

**Result:**

```
[
  {
    "EntryType": "Transfer",
    "JournalTemplateName": "TRANSFER",
    "JournalBatchName": "DEFAULT",
    "LineNo": 10000,
    "PostingDate": "2023-06-20",
    "DocumentNo": "PLU000001",
    "ItemNo": "1001",
    "UnitofMeasureCode": "PCS",
    "LocationCode": "EAST",
    "NewLocationCode": "MAIN",
    "Quantity": 1.0
  }
]
```
