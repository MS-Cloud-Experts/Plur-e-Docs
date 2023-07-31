**ProcessMethod**: Update_QtyToReturn_V1

**Description**:
Update_QtyToReturn_V1

The method used to update the Sale Lines in the Sales Return Order.

The idea of the method is to update the Return Qty to Receive in the Sales Return Order in the picking process of the items.

**Parameters**:

The values of this field will be treated as Integers, this being the following mapping:


- **Sales Document Typo Enum Values**

    **Value:** 0; "Quote"
    **Value:** 1; "Order" 
    **Value:** 2; "Invoice"
    **Value:** 3; "Credit Memo" 
    **Value:** 4; "Blanket Order" 
    **Value:** 5; "Return Order" 

 
-	**No** :Warehouse Put Away number.
-	**ItemNo** : Item No related.
-	**LineNo** : Number  Line.
-	**QtytoReturn** : Quantities

**Output**:  If successful, the same fields used in the input will be returned as output, but with the updated value of Return Qty to Receive

**Example:**

![image.png](/.attachments/image-423b21fb-8965-4856-8fe1-47502a937471.png)


**Request:**
```
{
  "ProcessMethod": "Update_QtyToReturn_V1",
  "Parameters": [
    {
      "SalesLine": [
        {
          "DocumentType": "5",
          "DocumentNo": "S-RETORD1002",
          "LineNo": "1000",
          "No": "1015",
          "QtytoReturn": "2"
        }
      ]
    }
  ]
}
```

**Ouput:**

```
{
  "SalesLine": [
    {
      "DocumentType": "Return Order",
      "DocumentNo": "S-RETORD1002",
      "LineNo": "1000",
      "No": "1015",
      "Quantity": 5.0,
      "QtytoReturn": 2.0,
      "OutstandingQty": 5.0
    }
  ]
}
```
![image.png](/.attachments/image-34fc9424-b360-41f5-9e2a-a5f02860f408.png)


**Errors:**
```

```

