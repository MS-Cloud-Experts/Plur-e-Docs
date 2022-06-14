**CalculateWhseAdjustment:**
This process Calculate adjustments in quantity based on the warehouse adjustment bin for each item in the journal. New lines are added for negative and positive quantities. Additionally, events were added that allow tracking affected LP.

In **Business Central** we find this process on the Item Journal page:
![image.png](/.attachments/image-b2614682-ed2b-42b6-9ca4-68522de2d1c1.png)

To run it via api these are the only 2 parameters:

**ItemNo:** Represents the item for which you want to calculate the differences, if you leave the field blank, it will calculate the differences for the entire inventory.
**PostingDate:** Posting date that will be reflected in the Warehouse Entries.


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

