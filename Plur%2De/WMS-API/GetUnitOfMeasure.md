**ProcessMethod**: GetUnitOfMeasure

**Description**:
This method allows to obtain all the units of measures configured in the Business Central

**Ouput**: 
-	**UnitOfMeasure**: An array of Units of Measures

**Example**:

Request:

`"jsonRequest":"{"ProcessMethod":"GetWarehouseEmployee","Parameters":[{}]}"`

Outputs:


```
{
  "UnitOfMeasure": [
    {
      "Code": "BOX",
      "LocationCode": "Box"
    },
    {
      "Code": "CAN",
      "LocationCode": "Can"
    },
    {
      "Code": "DAY",
      "LocationCode": "Day"
    },
    {
      "Code": "HOUR",
      "LocationCode": "Hour"
    },
    {
      "Code": "KG",
      "LocationCode": "Kilo"
    },
    {
      "Code": "KM",
      "LocationCode": "Kilometer"
    },
    {
      "Code": "MILES",
      "LocationCode": "Miles"
    },
    {
      "Code": "PACK",
      "LocationCode": "Pack"
    },
    {
      "Code": "PALLET",
      "LocationCode": "Pallet"
    },
    {
      "Code": "PCS",
      "LocationCode": "Piece"
    },
    {
      "Code": "TEST",
      "LocationCode": "ewewq"
    }
  ]
}
```


