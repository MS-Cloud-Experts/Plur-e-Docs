**ProcessMethod**: Calcule_Possible_LPChilds_From_WR_V2

**Description**:


**Input**:

**Parameters**: 
-	**LP_Pallet_No**: Represents the number of the LP Pallet that you want to calculate the possible children of LP Single.

**Ouput**:  


**Request**:

```
{
  "ProcessMethod": "Calcule_Possible_LPChilds_From_WR_V2",
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
    "DocumentNo": "LP-01127",
    "Quantity": 3.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01128",
    "Quantity": 3.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01129",
    "Quantity": 3.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01130",
    "Quantity": 1.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01130",
    "Quantity": 1.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01131",
    "Quantity": 1.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01131",
    "Quantity": 1.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01132",
    "Quantity": 1.0,
    "UnitofMeasureCode": "PCS"
  },
  {
    "DocumentNo": "LP-01132",
    "Quantity": 1.0,
    "UnitofMeasureCode": "PCS"
  }
]
```
![image.png](/.attachments/image-16a6bf67-670d-458c-a671-0ae2bfbd7436.png)

**Childs:**
![image.png](/.attachments/image-b70efa85-5a5f-4412-8c1b-3919e5b71657.png)
 

**Errors**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The LP Pallet Header does not exist"
  }
}
```



