**ProcessMethod**: Calcule_Possible_LPChilds_From_WR_V3

**Description**:


**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of the LP Pallet that you want to calculate the possible children of LP Single.

**Ouput**:  


**Request**:

```
{
  "ProcessMethod": "Calcule_Possible_LPChilds_From_WR_V3",
  "Parameters": [
    {
      "LP_Pallet_No": "LP-0000060"
    }
  ]
}
```


**Outputs**:


```
[
  {
    "BinCode": "REC-1",
    "DocumentType": "Whse. Journal",
    "ItemNo": "1013",
    "LocationCode": "NEWWMS",
    "LPDocumentNo": "LP-01182",
    "Quantity": 2.0,
    "SystemCreatedAt": "2023-04-05T19:20:22.6900000Z",
    "UnitofMeasure": "PCS"
  },
  {
    "BinCode": "REC-1",
    "DocumentType": "Whse. Journal",
    "ItemNo": "1013",
    "LocationCode": "NEWWMS",
    "LPDocumentNo": "LP-01183",
    "Quantity": 2.0,
    "SystemCreatedAt": "2023-04-05T19:20:49.2130000Z",
    "UnitofMeasure": "PCS"
  }
]
```

**Errors**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The LP Pallet Header does not exist"
  }
}
```



