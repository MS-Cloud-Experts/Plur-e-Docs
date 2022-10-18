
```
{
  "ProcessMethod": "Update_WarehousePutAway_Lines",
  "Parameters": [
    {
      "WarehousePutAwayLines": [
        {
          "ActivityType": 1,
          "No": "WHSE PUTAWAY-00021",
          "ItemNo": "1896-S",
          "LineNo": "20000",
          "ZoneCode": "STO",
          "LocationCode": "WMS",
          "BinCode": "FLOOR",
          "Quantity": 5.0,
          "LP": "LP-00144"
        },
        {
          "ActivityType": 1,
          "No": "WHSE PUTAWAY-00021",
          "ItemNo": "1896-S",
          "LineNo": "22500",
          "ZoneCode": "",
          "LocationCode": "WMS",
          "BinCode": "",
          "Quantity": 5.0,
          "LP": "LP-00143"
        },
        {
          "ActivityType": 1,
          "No": "WHSE PUTAWAY-00021",
          "ItemNo": "1896-S",
          "LineNo": "25000",
          "ZoneCode": "",
          "LocationCode": "WMS",
          "BinCode": "",
          "Quantity": 5.0,
          "LP": "LP-00142"
        },
        {
          "ActivityType": 1,
          "No": "WHSE PUTAWAY-00021",
          "ItemNo": "1896-S",
          "LineNo": "30000",
          "ZoneCode": "",
          "LocationCode": "WMS",
          "BinCode": "",
          "Quantity": 5.0,
          "LP": "LP-00141"
        }
      ]
    }
  ]
}
```

**Ouput:**

```
{
  "WarehousePutAwayLines": [
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "20000",
      "ZoneCode": "STO",
      "LocationCode": "WMS",
      "BinCode": "STO-1",
      "Quantity": 5.0,
      "LP": "LP-00144"
    },
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "22500",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 5.0,
      "LP": "LP-00143"
    },
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "25000",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 5.0,
      "LP": "LP-00142"
    },
    {
      "ActivityType": 1,
      "No": "WHSE PUTAWAY-00021",
      "ItemNo": "1896-S",
      "LineNo": "30000",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 5.0,
      "LP": "LP-00141"
    }
  ]
}
```



**Errors:**
```
{
  "error": {
    "code": "Internal_InvalidTableRelation",
    "message": "The field Bin Code of table Warehouse Activity Line contains a value (STO-01) that cannot be found in the related table (Bin).  CorrelationId:  33cccd63-b862-4ad6-b49a-6477225bf6da."
  }
}
```

