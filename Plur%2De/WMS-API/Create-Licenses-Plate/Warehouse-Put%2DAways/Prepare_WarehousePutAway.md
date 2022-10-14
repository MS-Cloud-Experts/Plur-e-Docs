**ProcessMethod**: Prepare_WarehousePutAway

**Description**:
This method returns the elements of the table "Warehouse Activity Header" filtered so that only "Put-Away" is visible. In this case, the filtered record is brought in the "No" field. returning the "Warehouse Activity Header" and the "Warehouse Activity Line" in JSON format.

Note: There is a table called " Warehouse Activity Header" which contains all registered Put-Aways and Pick, changing only the Type for differences between one or the other.

**Input**:
**Parameters**: 
-	**No**: Allows you to bring a single Warehouse Activity Header. 

**Ouput**:  

-	**WarehousePutAways**: Contains a Registered `WarehousePutAwayHeader` and an array of lines expressed in the key: `WarehouseActivityLine`.
-	
 
![image.png](/.attachments/image-16903ff2-59e0-411a-a940-09cf6dd2b617.png)


**Request:**

```
{
  "ProcessMethod": "Prepare_WarehousePutAway",
  "Parameters": [
    {
      "No": "WHSE PUTAWAY-00018"
    }
  ]
}
```


**Example**:





Outputs:

```
{
  "Post_Split": [
    {
      "LP": "LP-00123",
      "Qty": "5"
    },
    {
      "LP": "LP-00124",
      "Qty": "5"
    },
    {
      "LP": "LP-00125",
      "Qty": "5"
    },
    {
      "LP": "LP-00126",
      "Qty": "5"
    }
  ]
}
```

**Errors**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Put-Away does not exist""
  }
}
```

