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

**Outputs:**
 `"value": "Posted Batch Template: TRANSFER and Batch Name: DEFAULT"`

 `"value": "Created Batch Template: TRANSFER and Batch Name: DEFAULT"`

**Errors possible:**
 
```
"error": {
        "code": "Application_DialogException",
        "message": "You have insufficient quantity of Item 2000-S on inventory.  CorrelationId:  10b3fa85-1752-4f79-9836-33c6352b0995."
    }
```

```
"error": {
        "code": "Application_DialogException",
        "message": "Item No: 1896-S is managed by Plur-E. You must first create a License Plate for the Plur-E module and then attach it to the line before posting it. If it is already created, check that the status is 'Stored'  CorrelationId:  e63f74b6-64d4-4991-80fe-ebe33c276dbe."
    }
```

    
```
"error": {
        "code": "Internal_InvalidTableRelation",
        "message": "The field Item No. of table Item Journal Line contains a value (1000) that cannot be found in the related table (Item).  CorrelationId:  31a58348-194f-4615-9247-4fda58f0ec75."
    }
```

    
```
"error": {
        "code": "Application_DialogException",
        "message": "You must assign a lot number for item 1001. Line No. = '10000'.  CorrelationId:  378f7f4e-4edb-4682-9eca-4da02dfd8587."
    }
```




