**ProcessMethod**: Calcule_Possible_ItemChilds_From_WR

**Description**:
This method allows you to generate License Plates within Business Central associated with a Warehouse Receipt.

The output of this method returns the LP Document No Pallet Generated.

**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of the LP Pallet that you want to calculate the possible children of LP Single.

**Ouput**: List of LP Children candidates to be assigned to the LP Pallet.


**Request**:

```
{
  "ProcessMethod": "Calcule_Possible_ItemChilds_From_WR",
  "Parameters": [
    {
      "LP_Pallet_No": "LP-0000064"
    }
  ]
}
```


**Outputs**:

```
{
  "Possible_ItemsChilds": [
    {
      "LP": "1900-S",
      "Qty": "5"
    }
  ]
}
```
![image.png](/.attachments/image-dc0881dd-7cda-438c-9d09-43e5b44cbefd.png)

**Childs:**
![image.png](/.attachments/image-b72b953f-8dc8-4ae0-ab56-0294050a7b41.png)
 

**Errors**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The LP Pallet Header does not exist"
  }
}
```



