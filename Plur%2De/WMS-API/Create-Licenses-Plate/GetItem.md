**ProcessMethod**: GetItem

**Description**:
This method allows to obtain all the units of measures configured in the Business Central

**Ouput**: 
-	**UnitOfMeasure**: An array of Units of Measures

**Example**:

Request:


```
{
  "ProcessMethod": "GetItem",
  "Parameters": [
    {
      "ItemNo": "10s0"
    }
  ]
}
```


Outputs:


```
{
  "UnitOfMeasure": [
    {
      "Code": "BOX"
    },
    {
      "Code": "PALLET"
    },
    {
      "Code": "PCS"
    }
  ]
}
```
**Errors:**
`
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "There are no Units of Measure configured for product 10s0"
  }
}
`


