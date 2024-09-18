### Documentación de API: `PreRegister_WarehouseInvPhysicalCount`

#### **Visión General**
El método `PreRegister_WarehouseInvPhysicalCount` procesa las líneas del diario de inventario físico de un almacén, identificando y gestionando aquellas líneas que fueron sobrecontadas o subcontadas. Este método gestiona las placas de licencia (License Plates, LPs) y sus líneas relacionadas (padre-hijo), transfiriendo la información a un nuevo lote de diario para revisión, garantizando la integridad del inventario durante el proceso de conteo.

#### **Estructura de la Solicitud**
```json
{
  "ProcessMethod": "PreRegister_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "IVAN",
      "LocationCode": "NEWWMS",
      "WsheJournalBatchDobleCheckName": "IVAN-REVIEW"
    }
  ]
}
```

#### **Parámetros**
- **ProcessMethod**: El método a invocar, en este caso `"PreRegister_WarehouseInvPhysicalCount"`.
- **Parameters**: Un array de objetos que contiene los siguientes filtros:
  - **JournalTemplateName**: Nombre de la plantilla del diario de inventario (e.g., `"PHYSICAL I"`).
  - **JournalBatchName**: Nombre del lote del diario de inventario (e.g., `"IVAN"`).
  - **LocationCode**: Código de la ubicación del almacén (e.g., `"NEWWMS"`).
  - **WsheJournalBatchDobleCheckName**: Nombre del nuevo lote para la revisión de líneas (e.g., `"IVAN-REVIEW"`).

#### **Ejemplo de Solicitud**
```json
{
  "ProcessMethod": "PreRegister_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "IVAN",
      "LocationCode": "NEWWMS",
      "WsheJournalBatchDobleCheckName": "IVAN-REVIEW"
    }
  ]
}
```

#### **Ejemplo de Respuesta**
```json
{
  "WarehouseInvPhysicalCount_LP": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "IVAN",
      "BinCode": "10C3",
      "LineNo": 10000,
      "RegisteringDate": "2024-01-03",
      "LocationCode": "NEWWMS",
      "ItemNo": "1006",
      "UnitofMeasureCode": "PCS",
      "QtyPhysInventory": 1.0,
      "QtyCalculatedBase": 1.0,
      "UserID": "DARIO.SANCHEZ",
      "VariantCode": "",
      "SerialNo": "122112122",
      "LPDocumentNo": "LP-00123",
      "SuperParentLP": "LP-00123"
    },
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "IVAN",
      "BinCode": "10C3",
      "LineNo": 20000,
      "RegisteringDate": "2024-01-03",
      "LocationCode": "NEWWMS",
      "ItemNo": "1010",
      "UnitofMeasureCode": "PCS",
      "QtyPhysInventory": 3.0,
      "QtyCalculatedBase": 3.0,
      "UserID": "DARIO.SANCHEZ",
      "LPDocumentNo": "LP-00123",
      "SuperParentLP": "LP-00123"
    }
  ],
  "LPArray": [
    {
      "SuperParentLP": "LP-00123",
      "LPHierarchy": {
        "LPDocumentNo": "LP-00123",
        "LicensePlateStatus": "Stored",
        "ParentLPNo": "",
        "ZoneCode": "STO",
        "LocationCode": "NEWWMS",
        "BinCode": "10C3",
        "LPTotalQuantities": 4.0,
        "LPLines": [
          {
            "LineNo": 10000,
            "ItemNo": "1010",
            "Quantity": 3.0,
            "UnitofMeasure": "PCS"
          },
          {
            "LineNo": 20000,
            "ItemNo": "1006",
            "Quantity": 1.0,
            "UnitofMeasure": "PCS"
          }
        ],
        "ChildLPs": []
      }
    }
  ],
  "Duration": "450 milliseconds"
}
```

#### **Explicación**
- **WarehouseInvPhysicalCount_LP**: Un array que contiene los detalles del inventario físico contado en el almacén.
  - **JournalTemplateName**: Nombre de la plantilla del diario (e.g., `"PHYSICAL I"`).
  - **JournalBatchName**: Nombre del lote del diario (e.g., `"IVAN"`).
  - **BinCode**: El bin de almacenamiento donde se encuentran los artículos (e.g., `"10C3"`).
  - **LineNo**: El número de la línea dentro del lote del diario (e.g., `10000`).
  - **ItemNo**: Número de artículo (e.g., `"1006"`).
  - **QtyPhysInventory**: Cantidad que fue contada físicamente (e.g., `1.0`).
  - **QtyCalculatedBase**: Cantidad calculada según los datos del sistema (e.g., `1.0`).
  - **LPDocumentNo**: Número de documento de la placa de licencia (e.g., `"LP-00123"`).
  - **SuperParentLP**: El número de la placa de licencia principal (e.g., `"LP-00123"`).

- **LPArray**: Un array que contiene detalles sobre las placas de licencia (LPs) y su jerarquía.
  - **SuperParentLP**: La placa de licencia principal (e.g., `"LP-00123"`).
  - **LPHierarchy**: Detalles sobre la jerarquía de la placa de licencia.
    - **LPTotalQuantities**: Cantidad total asociada a la placa de licencia (e.g., `4.0`).
    - **LPLines**: Líneas asociadas a la placa de licencia.

#### **Resumen**
El método `PreRegister_WarehouseInvPhysicalCount` procesa las discrepancias de inventario físico, transfiriendo las líneas relacionadas con LPs a un nuevo lote para revisión y devolviendo información detallada en formato JSON. Este método maneja las relaciones entre placas de licencia (LPs) y asegura la integridad del sistema de inventario al agrupar las líneas de LPs padre e hijo.

### Lógica de Implementación
1. **Validación**:
   - Se validan parámetros como la plantilla del diario, el lote y la ubicación antes de procesar.

2. **Manejo de Lotes**:
   - Se crea o se recupera el lote para gestionar las discrepancias de LPs que fueron sobrecontados o subcontados.

3. **Procesamiento de Ajustes**:
   - Se identifican las líneas en el lote original que deben transferirse al lote de revisión, asegurando que las relaciones padre-hijo de los LPs sean manejadas correctamente.

4. **Eliminación de Líneas Originales**:
   - Las líneas del lote original se eliminan una vez que se han transferido al lote de revisión.

5. **Respuesta en JSON**:
   - Se genera una estructura JSON con los detalles de las líneas contadas y no contadas, proporcionando transparencia en el proceso de revisión de inventario.