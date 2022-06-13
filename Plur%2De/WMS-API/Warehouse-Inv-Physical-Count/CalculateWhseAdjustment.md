**CalculateWhseAdjustment:**
This process Calculate adjustments in quantity based on the warehouse adjustment bin for each item in the journal. New lines are added for negative and positive quantities. Additionally, events were added that allow tracking affected LP.


![image.png](/.attachments/image-b2614682-ed2b-42b6-9ca4-68522de2d1c1.png)

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

