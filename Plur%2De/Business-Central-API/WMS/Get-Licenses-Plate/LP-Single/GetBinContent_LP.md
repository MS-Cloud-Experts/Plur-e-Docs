**ProcessMethod**: GetBinContent_LP

**Description**:
This method allows obtaining the amounts associated by LP to a certain Item given the Location and the Bin.

The purpose of the method is to be able to use the [MoveBinToBin_LP](/Plur%2De/Business-Central-API/WMS/Movements/MoveBinToBin_LP) method properly.

**Input**:
**Parameters**: 
-	**BinCode**: Bin Code that you want to filter.
-	**LocationCode**: Location Code of the License Plate that you want to filter.
-	**ItemNo**: Item No of the License Plate that you want to filter.
-	**UnitofMeasureCode**: Unit of Measure Code of the License Plate that you want to filter.

**Ouput**: 
-	**TotalQty**: Total Items in Location/Bin.
-	**TotalQtyInLP**: Total Items in Location/Bin assigned to LP.
-	**Details**: An Array that breaks down the License Plates associated with the Items assigned to the location and their respective quantities.

Note: This will display relevant information on whether or not it is necessary to break an LP before performing the bin-to-bin move..


**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"GetBinContent_LP\",\"Parameters\":[{\"BinCode\":\"STO1\",\"LocationCode\":\"CCC\",\"ItemNo\":\"1900-S\",\"UnitofMeasureCode\":\"PCS\"}]}"`

Outputs:


```
{
  "TotalQty": 25.0,
  "TotalQtyInLP": 25.0,
  "Details": [
    {
      "LP": "LP000441",
      "Qty": "5"
    },
    {
      "LP": "LP000442",
      "Qty": "5"
    },
    {
      "LP": "LP000443",
      "Qty": "5"
    },
    {
      "LP": "LP000444",
      "Qty": "5"
    },
    {
      "LP": "LP000445",
      "Qty": "5"
    }
  ]
}
```
**Errors**:
```{
  "Error": {
    "Code": "Not found",
    "Message": "The Bin Code (STOa1) was not found"
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


