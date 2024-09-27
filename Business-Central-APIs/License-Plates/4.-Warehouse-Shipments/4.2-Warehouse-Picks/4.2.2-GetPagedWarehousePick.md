## Documentación de API: GetPagedWarehousePick

### Descripción General
El método `GetPagedWarehousePick` permite la obtención paginada de líneas de picks de almacén. Este enfoque es útil para manejar grandes volúmenes de datos al recuperar un número limitado de líneas por solicitud, lo que optimiza el rendimiento y facilita el procesamiento en lotes pequeños.

### Estructura de la Solicitud
```json
{
  "ProcessMethod": "GetPagedWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-03957",
      "Limit": 2,
      "Offset": 1
    }
  ]
}
```

### Parámetros
- **No**: El número del pick de almacén que se desea consultar (por ejemplo, `"WHSE PICK-03957"`).
- **Limit**: El número de líneas a recuperar por cada solicitud (por ejemplo, `2`).
- **Offset**: El punto de inicio desde el cual se van a recuperar las líneas, comenzando desde `1` (por ejemplo, `1`).

### Ejemplos de Solicitud y Respuesta

#### Primera Solicitud: Offset = 1
**Solicitud:**
```json
{
  "ProcessMethod": "GetPagedWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-03957",
      "Limit": 2,
      "Offset": 1
    }
  ]
}
```

**Respuesta:**
```json
{
  "Lines": [
    {
      "LineNo": 10000,
      "ItemNo": "DK21M22C",
      "VariantCode": "LS",
      "BinCode": "STORAGE"
    },
    {
      "LineNo": 20000,
      "ItemNo": "DK21M22C",
      "VariantCode": "LS",
      "BinCode": "SHIP"
    }
  ]
}
```

#### Segunda Solicitud: Offset = 2
**Solicitud:**
```json
{
  "ProcessMethod": "GetPagedWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-03957",
      "Limit": 2,
      "Offset": 2
    }
  ]
}
```

**Respuesta:**
```json
{
  "Lines": [
    {
      "LineNo": 30000,
      "ItemNo": "DK21M22C",
      "VariantCode": "LS",
      "BinCode": "STORAGE"
    },
    {
      "LineNo": 40000,
      "ItemNo": "DK21M22C",
      "VariantCode": "LS",
      "BinCode": "SHIP"
    }
  ]
}
```

### Explicación
- **Primera Solicitud (Offset = 1)**: Recupera las dos primeras líneas del pick (LineNo 10000 y 20000).
- **Segunda Solicitud (Offset = 2)**: Recupera las siguientes dos líneas (LineNo 30000 y 40000).

El parámetro `Offset` se utiliza para determinar el punto de inicio en las líneas que se van a recuperar, permitiendo la paginación y la obtención de diferentes lotes de datos en cada solicitud.

### Cálculo del Rango de Líneas
Para calcular el rango de líneas que se va a recuperar en función de los parámetros `Limit` y `Offset`, se puede utilizar la fórmula:
- **StartLine** = (Offset - 1) \* Limit \* 20000 + 10000
- **EndLine** = StartLine + Limit \* 20000 - 1

### Ejemplo de Respuesta Completa
**Respuesta de una Solicitud Completa:**
```json
{
  "WarehousePick": {
    "ShippingAgentCode": "UPS",
    "ShippingAgentServiceCode": "",
    "WarehousePickHeader": [
      {
        "No": "WHSE PICK-03957",
        "LocationCode": "MAIN",
        "AllowRegisterPick": true,
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "WILSON",
        "AssignmentDate": "2024-09-25",
        "CompletedbyPlure": false,
        "WarehousePickLines": [
          {
            "ActionType": "Take",
            "No": "WHSE PICK-03957",
            "WhseDocumentNo": "WHSE SHIP-04364",
            "LineNo": 30000,
            "ItemNo": "DK21M22C",
            "VariantCode": "LS",
            "SerialNo": "",
            "LotNo": "",
            "Description": "M CYCLONE ZF FULL 2/2MM LS",
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "SO-03001634",
            "SourceLineNo": 20000,
            "LocationCode": "MAIN",
            "BinCode": "14F5",
            "BinCodeList": [
              {"QtyAvailToTakeUOM": 4.0, "BinCode": "14F5"}
            ],
            "ZoneCode": "STORAGE",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "EA",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "ActionType": "Place",
            "No": "WHSE PICK-03957",
            "WhseDocumentNo": "WHSE SHIP-04364",
            "LineNo": 40000,
            "ItemNo": "DK21M22C",
            "VariantCode": "LS",
            "SerialNo": "",
            "LotNo": "",
            "Description": "M CYCLONE ZF FULL 2/2MM LS",
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "SO-03001634",
            "SourceLineNo": 20000,
            "LocationCode": "MAIN",
            "BinCode": "SHIP",
            "BinCodeList": [
              {"QtyAvailToTakeUOM": 4.0, "BinCode": "14F5"}
            ],
            "ZoneCode": "SHIP",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "EA",
            "QtyperUnitofMeasure": 1.0
          }
        ]
      }
    ],
    "ItemHasTrackingJA": [
      {"LineNo": 30000, "ItemNo": "DK21M22C", "TrackingCode": ""}
    ],
    "SerialAvailable": [[]],
    "LotAvailable": [[]]
  },
  "Duration": "520 milliseconds"
}
```

### Resumen
El método `GetPagedWarehousePick` permite la recuperación de líneas de pick de almacén de manera paginada, utilizando los parámetros `Limit` y `Offset` para controlar la cantidad y el rango de datos recuperados en cada solicitud. Este enfoque mejora la eficiencia al manejar grandes volúmenes de datos. Además, es posible obtener información adicional sobre los agentes de envío, líneas de productos con o sin tracking, y los seriales o lotes disponibles para los ítems involucrados en el proceso de pick.