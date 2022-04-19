**ProcessMethod**: WarehouseInvPhysicalCount

**Description**:
This method allows you to increase or decrease an Item with its associated LP into the inventory.

**Input**:
**Parameters**: 
-	**ZoneCode**: Number of LP you want to increase or decrease.
-	**BinCode**: Zoneof LP you want to increase or decrease.
-	**LocationCode**: Bin where the LP you want to increase or decrease is currently located.
-	**LocationCode**: LP Location.
-	**RegisteringDate**: Item you want to move.
-	**WhseDocumentNo**: Quantities that you want to increase or decrease of an Item and an associated LP..
-	**UnitofMeasureCode**: Unit of Measure Code of the License Plate that you want to to increase or decrease.

**Ouput**: 
-	**Posted**: If the output presents the Posted value, it implies that the inventory movement was generated correctly.


**Example**:

Request:

`jsonRequest":"{\"ProcessMethod\":\"WarehouseInvPhysicalCount\",\"Parameters\":[{\"ZoneCode\":\"STO\",\"BinCode\":\"\",\"LocationCode\":\"CCC\",\"RegisteringDate\":\"2022-04-19\",\"WhseDocumentNo\":\"DocumentNo\"}]}`

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


