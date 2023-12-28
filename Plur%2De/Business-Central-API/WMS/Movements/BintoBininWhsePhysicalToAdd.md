**Request:**

**FromBin:** Depende de si el Item tiene Serial o No. En caso de que no tenga, se debe disenar el proceso de obtencion de datos.

```
[
  {
    "JournalBatchName": "DARIO",
    "JournalTemplateName": "GENERAL",
    "ZoneCode": "STO",
    "LocationCode": "NEWWMS",
    "ToBin": "STO1",
    "FromBin": "STO2",
    "ItemChildArray": [
      {
        "ItemNo": "1900-S",
        "VariantCode": "XDSCFSD",
        "LotNo": "LOTT0001",
        "SerialNo": "S000000001",
        "Qty": 1,
        "UnitofMeasureCode": "PCS"
      },
      {
        "ItemNo": "1900-S",
        "VariantCode": "XDSCFSD",
        "LotNo": "LOTT0001",
        "SerialNo": "S000000001",
        "Qty": 1,
        "UnitofMeasureCode": "PCS"
      }
    ]
  }
]
```


