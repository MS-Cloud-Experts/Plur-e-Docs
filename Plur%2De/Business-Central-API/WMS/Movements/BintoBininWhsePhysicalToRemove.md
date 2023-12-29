**Method:** BintoBininWhsePhysicalToRemove

1. Preguntar al usuario si el producto que no encontro lo desea mover a **nocount**.

**Request:**

```
[
  {
    "JournalBatchName": "DARIO",
    "JournalTemplateName": "GENERAL",
    "ZoneCode": "STO",
    "LocationCode": "NEWWMS",
    "FromBin": "STO1",
    "ToBin": "NOCOUNT",
    "ItemChildArray": [
      {
        "LineNo": "10000",
        "ItemNo": "1900-S",
        "Qty": 1,
        "UnitofMeasureCode": "PCS"
      },
      {
        "LineNo": "20000",
        "ItemNo": "1900-S",
        "Qty": 1,
        "UnitofMeasureCode": "PCS"
      }
    ]
  }
]
```
 