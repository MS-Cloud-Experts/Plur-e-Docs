**ProcessMethod**: Calcule_Possible_LPChilds_From_WR

**Description**:
This method allows you to assign an existing LP Single as a child to an LP Pallet.

The result of this method returns 2 fields, one whether the result was successful or not and the other the number of child lps that could be assigned to the pallet.

**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of LP Pallets you want to allocate the possible children of the LP Single.
-	**WarehouseReceipt_No**:  Represents the Warehouse Receipt Number where the Pallet is located. This field is used as an extra validation to verify that the LP Pallet is actually included in the Warehouse Receipt.
-	**LP_Pallet_Child_No**: Represents the child LP Pallet number to be assigned to the LP Pallet.

**Ouput**: 
-	**IsProcessed**: Boolean variable that indicates if the process was successful or not.
-	**Remnant_LPChilds**: Number of LP Singles that could be candidates to assign to an LP Pallet.

**Request**:

```
{
  "ProcessMethod": "Assign_LPChild_to_LP_Pallet_From_WR",
  "Parameters": [
    {
      "LP_Pallet_No": "LP-0000064",
      "WarehouseReceipt_No": "WHSE REC-0000007",
      "LP_Pallet_Child_No": "LP-0000065"
    }
  ]
}
```


**Outputs**:


```
{
  "Possible_LPChilds": "LP-0000059|LP-0000063"
}
```
![image.png](/.attachments/image-16a6bf67-670d-458c-a671-0ae2bfbd7436.png)

**Childs:**
![image.png](/.attachments/image-b70efa85-5a5f-4412-8c1b-3919e5b71657.png)
 

**Errors**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The LP Pallet Header does not exist"
  }
}
```





