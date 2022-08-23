**ProcessMethod**: Delete_LPChild_to_LP_Pallet_From_WR

**Description**:
This method allows you to remove an existing LP Single as a child of an LP Pallet.

The result of this method returns 2 fields, one if the delete process was executed correctly and the other the number of secondary LPs that could be assigned to an LP Pallet

**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of LP Pallets that you want to eliminate possible children of the LP Single.
-	**WarehouseReceipt_No**:  Represents the Warehouse Receipt Number where the Pallet is located. This field is used as an extra validation to verify that the LP Pallet is actually included in the Warehouse Receipt.
-	**LP_Pallet_Child_No**: It represents the LP Child that will be removed from the LP Pallet.

**Ouput**: 
-	**IsProcessed**: Boolean variable that indicates if the process was successful or not.
-	**Remnant_LPChilds**: Number of LP Singles that could be candidates to assign to an LP Pallet.

**Request**:
```
{
  "ProcessMethod": "Delete_LPChild_to_LP_Pallet_From_WR",
  "Parameters": [
    {
      "LP_Pallet_No": "LP-0000121",
      "WarehouseReceipt_No": "WHSE REC-0000007",
      "LP_Pallet_Child_No": "LP-0000124"
    }
  ]
}
```


**Outputs**:

```
{
  "IsProcessed": false,
  "Remnant_LPChilds": "LP-0000124|LP-0000125|LP-0000126"
}
```


**Possible Errors**:

```
{
  "Error": {
    "Code": "Not deleted",
    "Message": "The License Plate you are trying to remove does not exist in the document."
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
    "Code": "Not inserted",
    "Message": "The LP Single you are trying to remove does not exist"
  }
}

{
  "Error": {
    "Code": "Not Found",
    "Message": "The LP Pallet does not exist"
  }
}
```





