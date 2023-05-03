**ProcessMethod**: Update_QtyToShip_SalesLines_V1

**Description**:
Update_QtyToShip_SalesLines_V1

The method used to update the Sale Lines in the Sales Order.

The idea of the method is to update the Qty to Ship in the Sales Order in the picking process of the items.

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
-	**Qty to Ship** : Quantities

**Output**:  If successful, the same fields used in the input will be returned as output, but with the updated value of Qty to ship

**Example:**

![image.png](/.attachments/image-b6faf901-f16e-461e-a33b-2ac9f14e37d1.png)


**Request:**
```
{
  "ProcessMethod": "Update_QtyToShip_SalesLines_V1",
  "Parameters": [
    {
      "SalesLine": [
        {
          "DocumentType": "1",
          "DocumentNo": "S-ORD101002",
          "LineNo": "10000",
          "No": "1968-S",
          "QtytoShip": "5"
        },
        {
          "DocumentType": "1",
          "DocumentNo": "S-ORD101002",
          "LineNo": "20000",
          "No": "1928-S",
          "QtytoShip": "3"
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
      "DocumentType": "Order",
      "DocumentNo": "S-ORD101002",
      "LineNo": "10000",
      "No": "1968-S",
      "Quantity": 10.0,
      "QtytoShip": 5.0,
      "OutstandingQty": 10.0
    },
    {
      "DocumentType": "Order",
      "DocumentNo": "S-ORD101002",
      "LineNo": "20000",
      "No": "1928-S",
      "Quantity": 7.0,
      "QtytoShip": 3.0,
      "OutstandingQty": 7.0
    }
  ]
}
```
![image.png](/.attachments/image-b4572646-4295-4ca0-8003-3fcdd3135a1d.png)


**Errors:**
```
{
    "error": {
        "code": "Application_DialogException",
        "message": "You cannot ship more than 10 units.  CorrelationId:  071b7020-d918-4d9d-aee9-8e476aadcdbd."
    }
}
```

