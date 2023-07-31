**ProcessMethod**: Calcule_Possible_LPChilds_From_WR

**Description**:
This method allows calculating the Possible Child LP Single that an LP Pallet could have in the Warehouse Receipt.

**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of the LP Pallet that you want to calculate the possible children of LP Single.

**Ouput**: List of LP Children candidates to be assigned to the LP Pallet.


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



