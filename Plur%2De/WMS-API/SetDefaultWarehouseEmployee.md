**ProcessMethod**: SetDefaultWarehouseEmployee

**Description**:
This method allows obtaining the amounts associated by LP to a certain Item given the Location and the Bin.

The purpose of the method is to be able to use the [MoveBinToBin_LP](/Plur%2De/WMS-API/MoveBinToBin_LP) method properly.

**Input**:
**Parameters**: 
-	**UserID**: Bin Code that you want to filter.
-	**LocationCode**: Location Code of the License Plate that you want to filter.
-	**Default**: Item No of the License Plate that you want to filter.

**Ouput**: 
-	**TotalQty**: Total Items in Location/Bin.
-	**TotalQtyInLP**: Total Items in Location/Bin assigned to LP.
-	**Details**: An Array that breaks down the License Plates associated with the Items assigned to the location and their respective quantities.

Note: This will display relevant information on whether or not it is necessary to break an LP before performing the bin-to-bin move..


**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"SetDefaultWarehouseEmployee\",\"Parameters\":[{\"UserID\":\"IVAN.LABRADOR1\",\"LocationCode\":\"MAIN WMS\",\"Default\":\"true\"}]}"`

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

{
  "Error": {
    "Code": "Not found",
    "Message": "The Item No (190a0-S) was not found"
  }
}
```


