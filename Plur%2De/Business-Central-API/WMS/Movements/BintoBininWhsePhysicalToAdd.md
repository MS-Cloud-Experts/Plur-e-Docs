**Request:**

**FromBin:** Depende de si el Item tiene Serial o No. En caso de que no tenga, se debe disenar el proceso de obtencion de datos.

```
{
  "ProcessMethod": "BintoBininWhsePhysicalToRemove",
  "Parameters": [
  {
    "JournalBatchName": "IVANL",
    "JournalTemplateName": "TEMPLATE",
    "ZoneCode": "STO",
    "LocationCode": "MAIN",
    "ToBin": "STO1",
    "FromBin": "NOCOUNT",
    "ItemChildArray": [
      {
        "ItemNo": "D0WHAREH",
        "VariantCode": "BLA00S",
        "LotNo": "",
        "SerialNo": "",
        "Qty": 10,
        "UnitofMeasureCode": "EA"
      }
    ]
  }
]
}
```

**Nota:** en caso de que el producto este en un inventario abierto NC deberia eliminarse de ahi tambien.


