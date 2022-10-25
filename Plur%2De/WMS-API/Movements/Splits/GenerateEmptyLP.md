**ProcessMethod**: GenerateEmptyLP

**Description**:
This method generates an empty License Plate, with the possibility of initializing it with a Location, Bin and Zone.

**Input**:
Parameters: 
-	ZoneCode: This parameter can be blank or specify an existing Zone Code..
-	LocationCode: This parameter can be blank or specify an existing Location Code.
-	BinCode: This parameter can be blank or specify an existing Bin Code.

**Ouput**: List of License Plates filtered by Item No.

-	**LPNo**: The Number of a newly created License Plate.

**Example**:

**Request**:
```
{
  "ProcessMethod": "GenerateEmptyLP",
  "Parameters": [
    {
      "ZoneCode": "STO",
      "LocationCode": "CCC",
      "BinCode": ""
    }
  ]
}
```

**OutPut:**


```
{
  "LPNo": "LP000776"
}
```

