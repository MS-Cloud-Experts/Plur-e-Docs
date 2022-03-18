**ProcessMethod**: MoveBinToBin_LP

**Description**:
Method that returns the combination of a License Plate Headers / License Plate Lines according to the number with which it is filtered.

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

`"jsonRequest":"{\"ProcessMethod\":\"MoveBinToBin_LP\",\"Parameters\":[{\"LPNo\":\"LP000445\",\"Zone\":\"STO\",\"FromBin\":\"STO2\",\"ToBin\":\"STO1\",\"LocationCode\":\"CCC\",\"ItemNo\":\"1900-S\",\"Qty\":\"5\",\"UnitofMeasureCode\":\"PCS\"}]}"`

Outputs:


```
{
  "Posted":212
}

```
**Errors**:
```{
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


