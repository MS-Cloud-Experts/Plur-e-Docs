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

**Business Central**

![image.png](/.attachments/image-f0c95d01-37c8-4cda-83db-9c78667eb727.png)


![image.png](/.attachments/image-9f9e11fc-f8ee-4602-b3a8-4fb253a0a248.png)
