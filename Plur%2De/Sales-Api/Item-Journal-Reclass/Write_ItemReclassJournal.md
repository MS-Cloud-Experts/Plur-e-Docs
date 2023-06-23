**Write_ItemReclassJournal:**
This method creates the lines of the Item Reclass.

If in the Plure configuration the auto reclass check is turned on, then at the time of writing it will be written and posted automatically.

![image.png](/.attachments/image-49025a53-995d-4fe3-b84a-fa30ef4e6b08.png)

In another scenario, only the lines will be created.



**Request:**

```
{
  "ProcessMethod": "Write_ItemReclassJournal",
  "Parameters": [
    {
      "Journal Template Name": "TRANSFER",
      "Journal Batch Name": "DEFAULT",
      "Line No": "10000",
      "Document No": "PLU000001",
      "Item No": "1000",
      "Location Code": "EAST",
      "New Location Code": "MAIN",
      "Quantity": "1",
      "Unit of Measure": "PCS"
    },
    {
      "Journal Template Name": "TRANSFER",
      "Journal Batch Name": "DEFAULT",
      "Line No": "20000",
      "Document No": "PLU000001",
      "Item No": "1000",
      "Location Code": "EAST",
      "New Location Code": "MAIN",
      "Quantity": "1",
      "Unit of Measure": "PCS"
    },
    {
      "Journal Template Name": "TRANSFER",
      "Journal Batch Name": "DEFAULT",
      "Line No": "30000",
      "Document No": "PLU000001",
      "Item No": "1000",
      "Location Code": "EAST",
      "New Location Code": "MAIN",
      "Quantity": "1",
      "Unit of Measure": "PCS"
    },
    {
      "Journal Template Name": "TRANSFER",
      "Journal Batch Name": "DEFAULT",
      "Line No": "40000",
      "Document No": "PLU000001",
      "Item No": "1000",
      "Location Code": "EAST",
      "New Location Code": "MAIN",
      "Quantity": "1",
      "Unit of Measure": "PCS"
    }
  ]
}
```

**Errors possible:**
 
```
"error": {
        "code": "Application_DialogException",
        "message": "You have insufficient quantity of Item 2000-S on inventory.  CorrelationId:  10b3fa85-1752-4f79-9836-33c6352b0995."
    }
```


