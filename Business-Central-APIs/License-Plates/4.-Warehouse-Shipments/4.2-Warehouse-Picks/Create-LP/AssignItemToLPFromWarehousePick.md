### API Documentation: AssignItemToLPFromWarehousePick

#### Overview
El método `AssignItemToLPFromWarehousePick` permite asignar múltiples artículos a License Plates (LPs) desde líneas de Warehouse Pick, con soporte opcional para tracking (Serial Numbers, Lot Numbers, y Expiration Dates). Este proceso es aplicable solo para artículos o variantes que no dispongan de LPs existentes en estado **Storage**, asegurando la unicidad de los LPs en almacenamiento. 

Esta funcionalidad mejorada soporta la asignación masiva de ítems y manejo de tracking, permitiendo una gestión de inventario más precisa y flexible.

#### Request Structure
```json
{
  "ProcessMethod": "AssignItemToLPFromWarehousePick",
  "Parameters": [
    {
      "PickNo": "PK-00025",
      "Items": [
        {
          "ItemNo": "ITEM001",
          "VariantCode": "VAR1",
          "QtyToPick": 5,
          "UnitofMeasureCode": "PCS",
          "PickLineNo": 10000,
          "Tracking": {
            "SerialNo": "SER001",
            "LotNo": "LOT001",
            "ExpirationDate": "2024-12-31"
          }
        },
        {
          "ItemNo": "ITEM002",
          "VariantCode": "",
          "QtyToPick": 10,
          "UnitofMeasureCode": "BOX",
          "PickLineNo": 20000
        }
      ]
    }
  ]
}
```

#### Parameters
- **PickNo**: Número del Warehouse Pick desde el cual se asignarán los artículos
- **Items**: Array de artículos a asignar, cada uno conteniendo:
  - **ItemNo**: Número de artículo (requerido)
  - **VariantCode**: Código de variante (opcional)
  - **QtyToPick**: Cantidad a recoger (requerido)
  - **UnitofMeasureCode**: Unidad de medida (requerido)
  - **PickLineNo**: Número de línea en el Warehouse Pick (requerido)
  - **Tracking**: Información de tracking (opcional)
    - **SerialNo**: Número de serie
    - **LotNo**: Número de lote
    - **ExpirationDate**: Fecha de caducidad

#### Example Response
```json
{
  "Details": [
    {
      "ItemNo": "ITEM001",
      "VariantCode": "VAR1",
      "Success": true,
      "LPDocumentNo": "LP-001",
      "AssignedQuantity": 5,
      "SerialNo": "SER001",
      "LotNo": "LOT001"
    },
    {
      "ItemNo": "ITEM002",
      "VariantCode": "",
      "Success": true,
      "LPDocumentNo": "LP-002",
      "AssignedQuantity": 10
    }
  ],
  "Message": "Items assignment to LP completed",
  "Duration": "2 seconds 456 milliseconds"
}
```

#### Response Fields
- **Details**: Array conteniendo el resultado de cada asignación:
  - **ItemNo**: Número de artículo procesado
  - **VariantCode**: Código de variante (si aplica)
  - **Success**: Indicador de éxito de la operación
  - **LPDocumentNo**: Número del LP asignado (en caso de éxito)
  - **AssignedQuantity**: Cantidad asignada
  - **SerialNo**: Número de serie (si se proporcionó)
  - **LotNo**: Número de lote (si se proporcionó)
  - **ErrorMessage**: Mensaje de error (en caso de fallo)

#### Error Response Example
```json
{
  "Details": [
    {
      "ItemNo": "ITEM001",
      "VariantCode": "VAR1",
      "Success": false,
      "ErrorMessage": "Cannot create new LP. Item ITEM001 Variant VAR1 already exists in LP LP-003 with Storage status. Please use existing LP."
    }
  ],
  "Message": "Items assignment to LP completed"
}
```

#### Validaciones
1. No se pueden crear LPs para items que ya tienen LPs en estado Storage
2. Las líneas de pick deben existir y no tener LPs asignados
3. La información de tracking debe ser válida según la configuración del ítem
4. Las cantidades deben ser positivas y estar dentro de las cantidades disponibles en la línea de pick

#### Casos de Uso Comunes
- Asignación masiva de items a LPs durante el proceso de picking
- Creación de LPs con tracking (serial/lot)
- Procesamiento de órdenes con múltiples items y variantes

#### Consideraciones Técnicas
- El proceso es transaccional: todas las asignaciones se procesan en una única transacción
- Se pueden procesar múltiples items en una sola llamada
- El tracking es opcional y se puede especificar por item
- Las respuestas incluyen información detallada para cada item procesado