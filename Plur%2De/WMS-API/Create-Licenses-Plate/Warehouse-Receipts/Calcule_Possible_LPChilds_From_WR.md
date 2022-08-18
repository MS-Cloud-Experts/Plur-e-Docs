**ProcessMethod**: Calcule_Possible_LPChilds_From_WR

**Description**:
This method allows you to generate License Plates within Business Central associated with a Warehouse Receipt.

The output of this method returns the LP Document No Pallet Generated.

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
  "ProcessMethod": "Calcule_Possible_LPChilds_From_WR",
  "Parameters": [
    {
      "LP_Pallet_No": "LP-0000060"
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



