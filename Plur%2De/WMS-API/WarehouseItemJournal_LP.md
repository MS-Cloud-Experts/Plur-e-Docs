**ProcessMethod**: WarehouseItemJournal_LP

**Description**:
This method allows you to move an Item with its associated LP into the inventory.

**Input**:
**Parameters**: 
-	**LPNo**: Number of LP you want to move.
-	**Zone**: Zoneof LP you want to move.
-	**FromBin**: Bin where the LP you want to move is currently located.
-	**ToBin**: Destination bin where you want to move the LP to..
-	**LocationCode**: LP Location.
-	**ItemNo**: Item you want to move.
-	**Qty**: QTY you want to move.
-	**UnitofMeasureCode**: Unit of Measure Code of the License Plate that you want to move.

**Ouput**: 
-	**Posted**: If the output presents the Posted value, it implies that the inventory movement was generated correctly.


**Example**:

Request:

`jsonRequest":"{\"ProcessMethod\":\"WarehouseItemJournal_LP\",\"Parameters\":[{\"LPNo\":\"LP000502\",\"Zone\":\"STO\",\"Bin\":\"STO2\",\"LocationCode\":\"BBB\",\"ItemNo\":\"1972-S\",\"Qty\":\"2\",\"UnitofMeasureCode\":\"PCS\"}]}`

Outputs:


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

