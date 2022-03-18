**ProcessMethod**: GetBinContent_LP

**Description**:
Method that returns the combination of a License Plate Headers / License Plate Lines according to the number with which it is filtered.

**Input**:
**Parameters**: 
-	**BinCode**: Number of the License Plate that you want to filter.
-	**LocationCode**: Number of the License Plate that you want to filter.
-	**ItemNo**: Number of the License Plate that you want to filter.
-	**UnitofMeasureCode**: Number of the License Plate that you want to filter.

**Ouput**: 
-	**LicensePlates**: Contains the information of a License Plate header in **LicensePlatesHeaders** and **LicensePlatesLines** contains an array of License Plate Lines.
-	
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
**Error**:
`{"Error":"The Licences Plate List is Empty"}`


