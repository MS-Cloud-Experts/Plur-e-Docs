**ProcessMethod**: GetWarehouseEmployee

**Description**:
Method that allows obtaining the list of Warehouse Employees with their respective locations.

**Ouput**: 
-	**WarehouseEmployees**: An array of users with their corresponding Location and whether or not it is default.
-	**UserID**: Represents the user ID.
-	**LocationCode**: Represents the location assigned to the user. 
-	**Default**: Represents if the location is configured as default for the user.


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


