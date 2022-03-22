**ProcessMethod**: GetBinContent_LP

**Description**:
This method allows obtaining the amounts associated by LP to a certain Item given the Location and the Bin.

The purpose of the method is to be able to use the [MoveBinToBin_LP](/Plur%2De/WMS-API/MoveBinToBin_LP) method properly.

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
  "WarehouseEmployees": [
    {
      "UserID": "GERMAN.GOMEZ",
      "LocationCode": "MAIN",
      "Default": false
    },
    {
      "UserID": "GERMAN.GOMEZ",
      "LocationCode": "PLUR-E M1",
      "Default": true
    },
    {
      "UserID": "GERMAN.GOMEZ 1",
      "LocationCode": "PLUR-E M1",
      "Default": true
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "AAA",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "ADVANCED1",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "BBB",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "CCC",
      "Default": true
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "EAST",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "MAIN WMS",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "PLUR-E M1",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR",
      "LocationCode": "WEST",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "AAA",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "ADVANCED1",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "BBB",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "CCC",
      "Default": true
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "EAST",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "MAIN WMS",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "PLUR-E M1",
      "Default": false
    },
    {
      "UserID": "IVAN.LABRADOR1",
      "LocationCode": "WEST",
      "Default": false
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


