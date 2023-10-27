**Request:**
```
{
  "ProcessMethod": "UpdateWarehousePickLines",
  "Parameters": [
    {
      "WhsDocumentNo": "WHSE PICK-00006",
      "PickLinesArray": [
        {
          "LineNo": 10000,
          "BincCode": "STO1",
          "VariantCode": "XLS",
          "SerialNo": "000001",
          "LotNo": "LOT10",
          "QtyToHandle": 1
        },
        {
          "LineNo": 30000,
          "BincCode": "STO1",
          "VariantCode": "XLS",
          "SerialNo": "000001",
          "LotNo": "LOT10",
          "QtyToHandle": 1
        },
      ]
    }
  ]
}
```

**OutPut:**

```


