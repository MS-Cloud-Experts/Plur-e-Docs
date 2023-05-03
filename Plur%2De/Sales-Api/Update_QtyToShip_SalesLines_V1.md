**ProcessMethod**: Update_QtyToShip_SalesLines_V1

**Description**:
Update_WarehousePutAway_Lines

The method used to update the Warehouse Put Away Lines or also known as Warehouse Activity Lines.

The idea of this method is to be able to be used before posting in case we want to update the destination of the Location/Bin of our LP.

**Input**:  The output is the information of new lines of a Warehouse Put Away, and although only the Key (Activity Type, Line No, No) is needed to perform any search, it has been decided to further detail the information with the following fields.

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

**Output**:  If successful, the same fields used in the input will be returned as output, but with the updated values of Bin, zone, and location.

**Example:**

![image.png](/.attachments/image-e368e677-2e16-4f5b-9cee-2faeb349800d.png)
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
          "DocumentNo": "S-ORD101001",
          "LineNo": "1000",
          "No": "1996-S",
          "QtytoShip": "6"
        },
        {
          "DocumentType": "1",
          "DocumentNo": "S-ORD101001",
          "LineNo": "11000",
          "No": "1900-S",
          "QtytoShip": "5"
        }
      ]
    }
  ]
}
```

**Ouput:**

```
{
  "WarehousePutAwayLines": [
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "20000",
      "ZoneCode": "STO",
      "LocationCode": "WMS",
      "BinCode": "STO-1",
      "Quantity": 5.0
    },
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "22500",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 5.0
    },
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "25000",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 5.0
    },
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "30000",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 5.0,
    }
  ]
}
```
![image.png](/.attachments/image-8e47e464-7a65-4e08-a120-0bd6ec91bd13.png)


**Errors:**
```
{
  "error": {
    "code": "Internal_InvalidTableRelation",
    "message": "The field Bin Code of table Warehouse Activity Line contains a value (STO-01) that cannot be found in the related table (Bin).  CorrelationId:  33cccd63-b862-4ad6-b49a-6477225bf6da."
  }
}

{
  "Error": {
    "Code": "Error Modifying",
    "Message": "Error modifying the Warehouse Activiy No WHSE PUTAWAY-000211, Line No 20000, Item No 1896-S, LP LP-00144"
  }
}
```

