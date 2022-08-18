**ProcessMethod**: DeleteLPPallet

**Description**:
This method allows you to Delete a License Plates associated to a Warehouse Receipt.

The output of this method returns the LP Document No Pallet removed and whether or not the removal was successful.

**Input**:

**Parameters**: 
-	**No**: Represents the number of the LP Pallet to remove.

**Ouput**: Returns 2 fields, one if it was successfully deleted, and another the number of the recently deleted LP Pallet.

-	**Delete**: Boolean value that indicates whether or not the executed process eliminated the LP Pallet.
-	**LPPallet_DocumentNo**: LP pallet number just removed.


**Request**:

```
{
  "ProcessMethod": "CreateLPPallet_FromWarehouseReceiptLine",
  "Parameters": [
    {
      "No": "WHSE REC-0000006",
      "ZoneCode": "REC",
      "LocationCode": "WMS",
      "BinCode": "REC-01"
    }
  ]
}
```


**Outputs**:


```
{
  "Created": true,
  "LPPallet_DocumentNo": "LP-0000062"
}
```

![image.png](/.attachments/image-df99e808-882a-4ee1-8a6b-7d46fdccb507.png)
 

**Errors**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The Warehouse Receipt Headers is empty"
  }
}


```



