**ProcessMethod**: Update_WsheReceiveLine

**Description**:

Method to update an Arrangement of Receipt Lines. Specially used to receive Items that are not handled by plur-e

**Parameters**:
 
-	**No** :Warehouse Receipt Number.
-	**SourceNo** :Source No.
-	**ItemNo** : Item No related.
-	**LineNo** : Number  Line.
-	**ZoneCode** : Zone
-	**LocationCode** : Location
-	**BinCode** : Bin
-	**QtyToReceive** : Qty To Receive

**Output**:  If successful, the same fields used in the input will be returned as output, but with the updated values of Bin, zone, and location.

**Example:**

![image.png](/.attachments/image-876de546-d238-4229-9c9a-e8553849a347.png)

**Request:**
```
{
  "ProcessMethod": "Update_WsheReceiveLine",
  "Parameters": [
    {
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00001",
          "SourceNo": "106006",
          "ItemNo": "1896-S",
          "LineNo": "10000",
          "ZoneCode": "STO",
          "LocationCode": "WMS",
          "BinCode": "REC-1",
          "QtyToReceive": 5.0
        },
        {
          "No": "WHSE REC-00001",
          "SourceNo": "106006",
          "ItemNo": "1900-S",
          "LineNo": "20000",
          "ZoneCode": "STO",
          "LocationCode": "WMS",
          "BinCode": "REC-1",
          "QtyToReceive": 5.0
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
      "No": "WHSE REC-00001",
      "ItemNo": "1896-S",
      "LineNo": "10000",
      "ZoneCode": "REC",
      "LocationCode": "WMS",
      "BinCode": "REC-1",
      "Quantity": 10.0,
      "QtyToReceive": 5.0
    },
    {
      "No": "WHSE REC-00001",
      "ItemNo": "1900-S",
      "LineNo": "20000",
      "ZoneCode": "REC",
      "LocationCode": "WMS",
      "BinCode": "REC-1",
      "Quantity": 10.0,
      "QtyToReceive": 5.0
    }
  ]
}
```
![image.png](/.attachments/image-46a82648-b51e-480f-b4a8-d45d1d600c0c.png)


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
    "Message": "Error modifying the Warehouse Receipt Line No WHSE REC-00001, Line No 20000, Item No 1896-S, QtyToReceive 5"
  }
}
```

