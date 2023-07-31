**ProcessMethod**: DeleteLPPallet

**Description**:
This method allows you to Delete a License Plates associated to a Warehouse Receipt.

The output of this method returns the LP Document No Pallet removed and whether or not the removal was successful.

**Note**: For now, LP Pallets can be removed if and only if they are still in the Warehouse Receipt.

**Input**:

**Parameters**: 
-	**No**: Represents the number of the LP Pallet to remove.

**Ouput**: Returns 2 fields, one if it was successfully deleted, and another the number of the recently deleted LP Pallet.

-	**Delete**: Boolean value that indicates whether or not the executed process eliminated the LP Pallet.
-	**LPPallet_DocumentNo**: LP pallet number just removed.


**Request**:

```
{
  "ProcessMethod": "DeleteLPPallet_FromWarehouseReceiptLine",
  "Parameters": [
    {
      "No": "LP-0000061"
    }
  ]
}
```


**Outputs**:


```
{
  "Deleted": true,
  "LPPallet_DocumentNo": "LP-0000061"
}
```


**Errors**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The LP Pallet does not exist"
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The LP Pallet is not assigned to a Warehouse Receipt, it cannot be deleted."
  }
}
```



