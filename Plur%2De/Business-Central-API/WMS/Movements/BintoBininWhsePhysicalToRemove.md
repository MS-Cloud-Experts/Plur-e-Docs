**Method:** BintoBininWhsePhysicalToRemove

1. Preguntar al usuario si el producto que no encontro lo desea mover a **Nocount**.

**Request:**
```
{
  "ProcessMethod": "BintoBininWhsePhysicalToRemove",
  "Parameters": [
    {
      "JournalBatchName": "IVANL",
      "JournalTemplateName": "TEMPLATE",
      "ZoneCode": "STO",
      "LocationCode": "MAIN",
      "FromBin": "STO1",
      "ToBin": "NOCOUNT",
      "ItemChildArray": [
        {
          "LineNo": "10000",
          "ItemNo": "D0WHAREH",
          "VariantCode" :"BLA00S",
          "Qty": 3,
          "UnitofMeasureCode": "EA",
          "LotNo": "",
          "SerialNo": ""
        }
      ]
    }
  ]
}
```

2. Crear un boton o proceso llamado preregister que lo que no se encontro lo mueva automaticamente al **NoCount**

- Se debe construir una API en BC o usar masivamente **BintoBininWhsePhysicalToRemove**.

- Enviar el listado de lo faltante al usuario. (o Estadisticas).

- Preguntar si todo el faltante lo quiere enviar a **NoCount**.
 