**Input**

```
{
  "ProcessMethod": "GetItemIdentifier",
  "Parameters": [
    {
      "ItemNo": "001"
    }
  ]
}
```


**OutPut**

```
{
  "ItemIdentifier": [
    {
      "Code": "001",
      "VariantCode": "BLACKL",
      "UnitofMeasureCode": "PCS"
    },
    {
      "Code": "002",
      "VariantCode": "BLACKM",
      "UnitofMeasureCode": "PCS"
    },
    {
      "Code": "003",
      "VariantCode": "BLACKS",
      "UnitofMeasureCode": "PCS"
    }
  ]
}
```



**Errors**

```
{
  "Error": "The ItemIdentifier ItemNo does not exist.",
  "ItemIdentifier": [
    {
      "Code": "",
      "VariantCode": "",
      "UnitofMeasureCode": ""
    }
  ]
}
```
