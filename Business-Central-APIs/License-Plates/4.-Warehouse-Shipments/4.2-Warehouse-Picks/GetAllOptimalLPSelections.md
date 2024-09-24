### API Documentation: GetAllOptimalLPSelections

#### **Overview**
El método `GetAllOptimalLPSelections` permite obtener una selección óptima de License Plates (LPs) para un proceso de Warehouse Pick, teniendo en cuenta la cantidad solicitada, la cantidad disponible en cada LP, y minimizando la necesidad de realizar divisiones (splits) o combinaciones innecesarias. Además, este método ya considera un enfoque **FEFO** (First Expired, First Out), priorizando los LPs con artículos que tengan la fecha de expiración más próxima.

#### **Request Structure**
```json
{
  "ProcessMethod": "GetAllOptimalLPSelections",
  "Parameters": [
    {
      "WarehousePickNo": "WHSE PICK-03610"
    }
  ]
}
```

#### **Parameters**
- **ProcessMethod**: El método a invocar, en este caso `"GetAllOptimalLPSelections"`.
- **Parameters**: Un array de objetos que describe los parámetros necesarios para la selección óptima de LPs.
  - **WarehousePickNo**: El número del Warehouse Pick, que sirve como identificador para las líneas de picking. (e.g., `"WHSE PICK-03610"`).

#### **Process Flow**
1. **Parseo de Parámetros**:
   - El sistema recibe un `JsonToken` que contiene el número del Warehouse Pick. Este parámetro es validado y extraído para su uso.

2. **Selección de LPs**:
   - Se recupera el inventario para identificar los LPs disponibles que coincidan con el `WarehousePickNo` proporcionado.
   - Los LPs se clasifican basándose en las siguientes prioridades:
     - **Cantidad en LP**: Los LPs con cantidades más cercanas a la solicitada.
     - **Fecha de expiración**: Los LPs con la fecha de expiración más próxima (FEFO).
     - **Ubicación en el almacén**: Se priorizan LPs más accesibles en bins mejor clasificados.

3. **Respuesta en JSON**:
   - La salida es un objeto JSON que contiene la selección óptima de LPs para cada línea de Warehouse Pick, incluyendo detalles sobre la cantidad disponible, la cantidad solicitada y si es necesario hacer un split.

#### **Example Request**
```json
{
  "ProcessMethod": "GetAllOptimalLPSelections",
  "Parameters": [
    {
      "WarehousePickNo": "WHSE PICK-03610"
    }
  ]
}
```

#### **Example Response**
```json
[
  {
    "PickNo": "WHSE PICK-03610",
    "ItemNo": "ITEM SERIAL TEST",
    "VariantCode": "",
    "LocationCode": "MAIN",
    "BinCode": "BACK",
    "UnitofMeasureCode": "EA",
    "LP": "LP-00023",
    "QtyInLP": 1.0,
    "QtyToTake": 1.0,
    "QtyRequested": 3.0,
    "NeedToSplit": true,
    "SufficientToFulfill": false,
    "ExpirationDate": "2024-01-15"
  },
  {
    "PickNo": "WHSE PICK-03610",
    "ItemNo": "ITEM SERIAL TEST",
    "VariantCode": "",
    "LocationCode": "MAIN",
    "BinCode": "BACK",
    "UnitofMeasureCode": "EA",
    "LP": "LP-00023",
    "QtyInLP": 1.0,
    "QtyToTake": 1.0,
    "QtyRequested": 3.0,
    "NeedToSplit": true,
    "SufficientToFulfill": false,
    "ExpirationDate": "2024-01-20"
  },
  {
    "PickNo": "WHSE PICK-03610",
    "ItemNo": "D0AVESVTBLU00S",
    "VariantCode": "",
    "LocationCode": "MAIN",
    "BinCode": "BACK",
    "UnitofMeasureCode": "EA",
    "LP": "LP-00023",
    "QtyInLP": 5.0,
    "QtyToTake": 2.0,
    "QtyRequested": 2.0,
    "NeedToSplit": false,
    "SufficientToFulfill": true,
    "ExpirationDate": "2023-12-10"
  }
]
```

#### **Response Fields**
- **PickNo**: Número del Warehouse Pick (e.g., `"WHSE PICK-03610"`).
- **ItemNo**: Número del artículo en el LP (e.g., `"ITEM SERIAL TEST"`).
- **VariantCode**: Código de variante del artículo, si aplica.
- **LocationCode**: Código de la ubicación del almacén (e.g., `"MAIN"`).
- **BinCode**: Código del bin donde se encuentra el LP (e.g., `"BACK"`).
- **UnitofMeasureCode**: Unidad de medida del artículo (e.g., `"EA"`).
- **LP**: Número del License Plate (LP) seleccionado (e.g., `"LP-00023"`).
- **QtyInLP**: Cantidad disponible en el LP (e.g., `1.0`).
- **QtyToTake**: Cantidad a tomar del LP para el Warehouse Pick (e.g., `1.0`).
- **QtyRequested**: Cantidad solicitada en la línea del Warehouse Pick (e.g., `3.0`).
- **NeedToSplit**: Indica si es necesario dividir el LP para cumplir con la cantidad solicitada (e.g., `true`).
- **SufficientToFulfill**: Indica si el LP tiene suficiente cantidad para cumplir con la solicitud sin necesidad de splits (e.g., `false`).
- **ExpirationDate**: Fecha de expiración del artículo en el LP (e.g., `"2024-01-15"`).

#### **Consideraciones del Algoritmo FEFO**
El algoritmo de selección de LPs sigue el enfoque **FEFO (First Expired, First Out)**, priorizando aquellos LPs que contienen artículos con fechas de expiración más cercanas, garantizando que los artículos perecederos o sensibles al tiempo sean utilizados primero.

- **Validación de Fecha de Expiración**: Cada LP es revisado para obtener la fecha de expiración del artículo, y aquellos con fechas más cercanas son priorizados.
- **Evitar Split innecesarios**: Si existen múltiples LPs con cantidades similares, el sistema selecciona el LP con la fecha de expiración más cercana para minimizar la fragmentación.

#### **Process Logic**
1. **Validación**:
   - El Warehouse Pick es validado para asegurar que todas las líneas estén en un estado válido y que los LPs estén disponibles en el almacén.
   
2. **Selección Óptima**:
   - El algoritmo selecciona los LPs priorizando las cantidades más cercanas a las solicitadas y los artículos con fechas de expiración más cercanas (FEFO).
   - En caso de que la cantidad en el LP no sea suficiente, el campo `NeedToSplit` se activa, indicando la necesidad de dividir el LP.

3. **Actualización en Tiempo Real**:
   - A medida que se realiza la selección de LPs, los estados se actualizan en tiempo real en el sistema para mantener la trazabilidad del inventario.

#### **Example Output with FEFO**
```json
[
  {
    "PickNo": "WHSE PICK-03610",
    "ItemNo": "ITEM01",
    "LocationCode": "MAIN",
    "LP": "LP-00001",
    "QtyInLP": 5.0,
    "QtyToTake": 3.0,
    "ExpirationDate": "2023-11-01",
    "NeedToSplit": false
  },
  {
    "PickNo": "WHSE PICK-03610",
    "ItemNo": "ITEM01",
    "LocationCode": "MAIN",
    "LP": "LP-00002",
    "QtyInLP": 2.0,
    "QtyToTake": 2.0,
    "ExpirationDate": "2023-12-01",
    "NeedToSplit": true
  }
]
```

#### **Summary**
El método `GetAllOptimalLPSelections` ofrece una solución avanzada para la selección de License Plates en el contexto de Warehouse Pick, incorporando lógica de **FEFO** para garantizar que los artículos con fechas de expiración más cercanas se seleccionen primero. El proceso minimiza las divisiones de LPs y asegura la trazabilidad y precisión en la gestión de inventario.