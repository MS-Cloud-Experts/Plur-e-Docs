**ProcessMethod**: WarehouseInvPhysicalCount

**Description**:
This method allows you to increase or decrease an Item with its associated LP into the inventory.

**Input**:
**Parameters**: 
-	**ZoneCode**: Specific Zone where you want to perform the inventory count.
-	**BinCode**: Specific Bin where you want to perform the inventory count.
-	**LocationCode**: Specific Location where you want to perform the inventory count.
-	**RegisteringDate**: Item you want to move.
-	**WhseDocumentNo**:

**Ouput**: 
-	**Posted**: If the output presents the Posted value, it implies that the inventory movement was generated correctly.


**Example**:

Request:

`jsonRequest":"{\"ProcessMethod\":\"Create_WarehouseInvPhysicalCount\",\"Parameters\":[{\"ZoneCode\":\"STO\",\"BinCode\":\"\",\"LocationCode\":\"CCC\",\"RegisteringDate\":\"2022-04-19\",\"WhseDocumentNo\":\"DocumentNo\"}]}`

**Outputs**:


```
{
  "Posted":212
}
```

**Errors**:
```
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The item 1972-S is not managed by the Plur-e WMS module. If you want to configure it, you must go to the Item Card and turn on the check 'Managed by Plur-E'"
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The License Plate is already in the specified location and bin."
  }
}

{
  "Error": {
    "Code": "Not found",
    "Message": "The Location Code (CCCa) was not found"
  }
}

{
  "Error": {
    "Code": "Not found",
    "Message": "The Item No (190a0-S) was not found"
  }
}
```


