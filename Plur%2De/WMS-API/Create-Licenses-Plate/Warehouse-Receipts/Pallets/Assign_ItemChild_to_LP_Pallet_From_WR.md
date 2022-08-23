**ProcessMethod**: Assign_ItemChild_to_LP_Pallet_From_WR

**Description**:
This method allows you to assign a Warehouse Receipt Item as a child to an LP Pallet.

The result of this method returns 2 fields, one whether the result was successful or not and the other the number of child lps that could be assigned to the pallet.

**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of LP Pallets you want to allocate the possible children of the LP Single.
-	**WarehouseReceipt_No**:  Represents the Warehouse Receipt Number where the Pallet is located. This field is used as an extra validation to verify that the LP Pallet is actually included in the Warehouse Receipt.
-	**Item_Child_No**: Item number to assign.
-	**Qty**: Quantities available to assign.
-	**WarehouseReceipt_LineNo**: It represents the line corresponding to the Warehouse Receipt that contains the Item that you want to assign to the LP Pallet. This information is important because a Warehouse Receipt could have a Repeated Item.

**Ouput**: 
-	**IsProcessed**: Boolean variable that indicates if the process was successful or not.
-	**Possible_ItemsChilds**: Json array with possible Items to be assigned to a License Plate Pallet.

This Arrangement contains:

  **"No"**: Warehouse Recetip number, example: "WHSE REC-0000007".
  **"Line No"**: Number of the line where the Item is in the Warehouse Recipe. Necessary to locate you at the time of being assigned. Example: 10000.
  **"Item No"**: Item number available. Example: "1896-S".
  **"Qty"**: Quantities available to assign. Example: 5.0.

**Request**:
```
{
  "ProcessMethod": "Assign_ItemChild_to_LP_Pallet_From_WR",
  "Parameters": [
    {
      "LP_Pallet_No": "LP-0000121",
      "WarehouseReceipt_No": "WHSE REC-0000007",
      "Item_Child_No": "1900a-S",
      "Qty": "5",
      "WarehouseReceipt_LineNo": "20000"
    }
  ]
}
```


**Outputs**:

```
{
  "IsProcessed": true,
  "Possible_ItemsChilds": [
    {
      "No": "WHSE REC-0000007",
      "Line No": 10000,
      "Item No": "1896-S",
      "Qty": 5.0
    }
  ]
}
```

![image.png](/.attachments/image-6675877d-9126-40b7-be52-836af42197bc.png) 


**Possible Errors**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": "Error in the parameters, or the Item you are trying to send is already assigned to the License Plate Pallet"
  }
}

{
  "Error": {
    "Code": "Not Found",
    "Message": "The Warehouse Receipt No. does not match the LP Pallet Document No."
  }
}

{
  "Error": {
    "Code": "Not Found",
    "Message": "The Item No= 1900A-S you are trying to assign does not exist"
  }
}
```





