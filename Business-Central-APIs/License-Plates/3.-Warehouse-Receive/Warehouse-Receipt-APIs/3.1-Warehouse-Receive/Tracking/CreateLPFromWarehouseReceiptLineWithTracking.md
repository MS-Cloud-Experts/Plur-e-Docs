### Documentación de la API: CreateLPFromWarehouseReceiptLineWithTracking

#### Descripción
Este proceso de API permite crear *N* LPs (License Plates) según el valor especificado en el parámetro `TotalToReceive`. La cantidad de LPs creados debe coincidir con el número de elementos presentes en el array `TrackingInfo`. Cada LP creado contendrá una sola línea con la información específica de seguimiento proporcionada.

**Nota**: Si se desea crear múltiples líneas en un único LP, por favor refiérase al [API AssignItemToLPWithTracking](https://dev.azure.com/MSCloudExperts/Plur-e/_wiki/wikis/Plur-e.wiki/458/AssignItemToLPWithTracking).

#### Estructura de la Solicitud
```json
{
  "ProcessMethod": "CreateLPFromWarehouseReceiptLineWithTracking",
  "Parameters": [
    {
      "No": "WHSE REC-00186",
      "ItemNo": "K3CSODQL",
      "BinCode": "MAIN",
      "LineNo": 10000,
      "UnitofMeasureCode": "PCS",
      "TotalToReceive": 3,
      "PackUnitUoM": "BOX",
      "TrackingInfo": [
        {
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN002",
          "LotNo": "LOT002",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN003",
          "LotNo": "LOT003",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        }
      ]
    }
  ]
}
```

#### Ejemplo de Solicitud
```json
{
  "ProcessMethod": "CreateLPFromWarehouseReceiptLineWithTracking",
  "Parameters": [
    {
      "No": "WHSE REC-0001",
      "ItemNo": "ITEM-001",
      "BinCode": "BIN-01",
      "LineNo": 10000,
      "UnitofMeasureCode": "PCS",
      "TotalToReceive": 3,
      "PackUnitUoM": "BOX",
      "TrackingInfo": [
        {
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN002",
          "LotNo": "LOT002",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN003",
          "LotNo": "LOT003",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        }
      ]
    }
  ]
}
```

#### Ejemplo de Respuesta
```json
{
  "WarehouseReceiptNo": "WHSE REC-00186",
  "ItemNo": "K3CSODQL",
  "LineNo": 10000,
  "VariantCode": "NMEDXXX",
  "TrackingSpecificationOpen": [
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN001",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN002",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN003",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    }
  ],
  "LP_Pending_To_Receive": 997.0,
  "LP_Received": "LP-00073-10000|LP-00074-10000|LP-00075-10000",
  "Message": "The LPs were created successfully with tracking.",
  "Duration": "16 seconds 951 milliseconds"
}
```

#### Explicación
- **WarehouseReceiptNo**: `"WHSE REC-00186"` - Número de recibo de almacén para el cual se están creando los LPs.
- **ItemNo**: `"K3CSODQL"` - Número de ítem asociado con la línea del recibo de almacén.
- **LineNo**: `10000` - Número de línea del recibo de almacén.
- **UnitofMeasureCode**: `"PCS"` - Código de la unidad de medida de los ítems.
- **TrackingInfo**: Array que contiene la información de seguimiento de los ítems, donde cada ítem está representado con un `SerialNo`, `LotNo`, y `ExpirationDate` únicos. Cada entrada también incluye la cantidad (`Qty`) para ese ítem específico.

#### Resumen
En este ejemplo simplificado, la API maneja un caso donde se reciben tres unidades de un ítem, cada una con un número de serie único y un número de lote único, asegurando el seguimiento y la identificación adecuados dentro del almacén. El array `TrackingInfo` contiene entradas individuales para cada unidad, cada una especificando una cantidad de 1, lo que hace que el proceso sea directo y fácil de entender. Este enfoque es ideal para gestionar inventarios serializados donde cada ítem necesita ser rastreado individualmente.

### Consideraciones Adicionales
- **Creación de LPs Individuales:** Este método crea un LP por cada unidad recibida con su respectivo `SerialNo`, lo que es esencial para rastrear artículos con números de serie únicos.
- **Referencia a Otros Métodos:** Si necesitas crear múltiples líneas en un solo LP en lugar de un LP por cada ítem, consulta la documentación para el método [AssignItemToLPWithTracking](https://dev.azure.com/MSCloudExperts/Plur-e/_wiki/wikis/Plur-e.wiki/458/AssignItemToLPWithTracking).