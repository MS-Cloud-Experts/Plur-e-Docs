
**JsonRequest:**
```
{
  "ProcessMethod": "CalculateWhseAdjustment",
  "Parameters": [
    {
      "ItemNo": "1900-S",
      "PostingDate": "2022-04-19"
    }
  ]
}
```



**Result:**
```
{
  "Result_CalculateWhseAdjustment": [
    {
      "JournalBatchName": "PLUR-E",
      "JournalTemplateName": "ITEM",
      "DocumentNo": "D-00001",
      "LineNo": 10000,
      "ItemNo": "1900-S",
      "LP": "LP-0000015",
      "Qty": 1.0,
      "Amount": 150.3
    }
  ]
}
```

**Errors:**

```
{
  "Error": {
    "Code": "Not Created",
    "Message": "No element with the given parameters were found in the process of Calculate Whse. Adjustment"
  }
}
```

