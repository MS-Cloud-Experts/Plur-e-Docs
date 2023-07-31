**GetItemIdentifier**

![image.png](/.attachments/image-08bf5a3a-7e89-4694-abfd-17fef9de4a10.png)

**Input**

```
{
  "ProcessMethod": "GetItemIdentifier",
  "Parameters": [
    {
      "Code": "001"
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
