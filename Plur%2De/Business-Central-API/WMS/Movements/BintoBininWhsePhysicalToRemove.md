**Method:** BintoBininWhsePhysicalToRemove

1. Preguntar al usuario si el producto que no encontro lo desea mover a **Nocount**.

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
        "UnitofMeasureCode": "PCS",
        "LotNo": "LOTT0001",
        "SerialNo": "S000000001",
      },
      {
        "LineNo": "20000",
        "ItemNo": "1900-S",
        "Qty": 1,
        "UnitofMeasureCode": "PCS",
        "LotNo": "LOTT0001",
        "SerialNo": "S000000001",
      }
    ]
  }
]
```

2. Crear un boton o proceso llamado preregister que lo que no se encontro lo mueva automaticamente al **NoCount**
 