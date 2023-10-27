**Request:**
```
{
  "ProcessMethod": "CreatePackageShipment",
  "Parameters": [
    {
      "WhsDocumentNo": "WHSE PICK-00006",
      "PickLinesArray": [
        {
          "LineNo": 20000,
          "BincCode": "STO1",
          "VariantCode": "XLS",
          "SerialNo": "000001",
          "LotNo": "LOT10",
          "QtyToHandle": 1
        },
        {
          "LineNo": 40000,
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


