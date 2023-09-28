**Ouput:**

**Request:**
```
{
  "ProcessMethod": "GetBinContentV2",
  "Parameters": [
    {
      "BinCode": "STO-3",
      "LocationCode": "NEWWMS",
      "ItemNo": "1900-S",
      "UnitofMeasureCode": "PCS"
    }
  ]
}
```

**OutPut:**
```
{
  "ItemNo": "1900-S",
  "LocationCode": "NEWWMS",
  "BinCode": "STO-3",
  "ItemQty": [
    {
      "ItemNo": "1900-S",
      "Qty": 10325.0,
      "QtyAvailToTakeUOM": 10273.0,
      "CalcQtyAvailToPick": 10273.0,
      "CalcQtyAvailToPutAway": -10325.0
    }
  ],
  "QtyXVariants": []
}
```

![image.png](/.attachments/image-6a4dedbb-8e22-4f18-a435-8ccf72e220a5.png)
