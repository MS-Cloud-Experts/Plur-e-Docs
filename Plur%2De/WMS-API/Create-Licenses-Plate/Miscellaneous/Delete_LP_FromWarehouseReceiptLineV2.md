**Request:**

**Document Type:**
    
```
value(0; "Single") { Caption = 'Single'; }
value(1; "Pallet") { Caption = 'Pallet'; }
value(2; " ") { Caption = ''; }
```


```
{
  "ProcessMethod": "Delete_LP_FromWarehouseReceiptLineV2",
  "Parameters": [
    {
      "LPChildArray": [
        {
          "LPDocumentNo": "LP-01096",
          "LPDocumentType": 1
        },
        {
          "LPDocumentNo": "LP-01097",
          "LPDocumentType": 1
        },
        {
          "LPDocumentNo": "LP-01097",
          "LPDocumentType": 0
        },
      ]
    }
  ]
}
```
