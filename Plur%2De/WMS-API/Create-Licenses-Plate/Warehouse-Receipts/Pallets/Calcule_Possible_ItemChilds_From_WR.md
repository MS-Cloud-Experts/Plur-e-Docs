**ProcessMethod**: Calcule_Possible_ItemChilds_From_WR

**Description**:
This method allows calculating the Possible Child Items that an LP Pallet could have in the Warehouse Receipt.

The output is a json array with the Item No / Available Outstanding Quantities value pair.

**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of LP Pallets that you want to calculate the possible Child Items in a Warehouse Receipt.

**Ouput**: Json array with the Items and quantities available.


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



