**ProcessMethod**: DeleteLPPallet

**Description**:
This method allows you to Delete a License Plates associated to a Warehouse Receipt.

The output of this method returns the LP Document No Pallet removed and whether or not the removal was successful.

**Input**:

**Parameters**: 
-	**No**: Represents the Warehouse Receipt number to which you want to assign a LP. 
-	**BinCode**: Bin Code assigned to the product in the Warehouse Receipt.
-	**LocationCode**: Unit of measure assigned to the product in the Warehouse Receipt.
-	**ZoneCode**: Total number to receive expressed in the base unit of measure.

**Ouput**: Method that returns the number of assigned and pending LP to be assigned to a Warehouse Receipt.

-	**Created**: Boolean value that indicates if the process that was executed created a new License Plate. 
-	**LPPallet_DocumentNo**: Newly created LP Pallet number..


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



