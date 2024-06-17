**Request:**
```
{
  "ProcessMethod": "GetInventoyByItemNo",
  "Parameters": [
    {
      "ItemNo": "D1WHLFIH",
      "VariantCode": "DLA028",
      "LocationCode": "ASIA"
    }
  ]
}
```
**Ouput:**

```
{
  "InventoryByItemNo": [
    {
      "ItemNo": "D1WHLFIH",
      "VariantCode": "DLA028",
      "LocationCode": "ASIA",
      "Description": "FIXED LINES",
      "UnitofMeasureCode": "EA",
      "Quantity": 407.0
    }
  ],
  "Duration": "114 milliseconds"
}
```
