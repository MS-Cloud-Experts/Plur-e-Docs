### API Documentation: GetAllOptimalLPSelections

#### **Overview**
El método `GetAllOptimalLPSelections` permite obtener una selección optimizada de License Plates (LPs) para un proceso de **Warehouse Pick** en función de las cantidades solicitadas y disponibles, la necesidad de división (split), y un criterio de **prioridad**. El sistema utiliza un **PriorityScore** basado en una serie de reglas refinadas que consideran la exactitud de las cantidades solicitadas, la existencia de ítems adicionales, y si las cantidades son suficientes o no.

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
  - **WarehousePickNo**: El número del Warehouse Pick que se está procesando. (e.g., `"WHSE PICK-03610"`).

#### **Process Flow**
1. **Parseo de Parámetros**:
   - Se valida y extrae el número de Warehouse Pick para identificar las líneas de picking relacionadas.

2. **Selección de LPs**:
   - El sistema obtiene todos los LPs disponibles que coincidan con el `WarehousePickNo`.
   - Los LPs se clasifican según las cantidades solicitadas, las cantidades disponibles en los LPs, y si es necesario hacer un split.
   - Se calcula un **PriorityScore** para cada LP en función de las siguientes reglas:

     - **PriorityScore = 1**: Cantidad exacta sin ítems extra.
     - **PriorityScore = 2**: Cantidad exacta, pero con ítems adicionales.
     - **PriorityScore = 3**: Cantidad suficiente o superior sin ítems extra.
     - **PriorityScore = 4**: Cantidad suficiente o superior, pero con ítems adicionales.
     - **PriorityScore = 5**: Cantidad insuficiente, sin ítems adicionales.
     - **PriorityScore = 6**: Cantidad insuficiente, con ítems adicionales.

3. **Salida en JSON**:
   - La salida es un objeto JSON que contiene la selección óptima de LPs para cada línea del Warehouse Pick, junto con el **PriorityScore**, las cantidades disponibles y solicitadas, y si es necesario hacer un split.

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
{
  "LPOPtimalSelections": [
    {
      "PickNo": "WHSE PICK-03610",
      "ItemNo": "ITEM SERIAL TEST",
      "VariantCode": "",
      "SerialNo": "1",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "LocationCode": "MAIN",
      "BinCode": "BACK",
      "UnitofMeasureCode": "EA",
      "LP": "LP-00023",
      "PriorityScore": 4.0,
      "QtyInLP": 1.0,
      "QtyToTake": 1.0,
      "QtyOrignalRequested": 3.0,
      "QtyRemaingRequested": 3.0,
      "NeedToSplit": true,
      "SufficientToFulfill": false
    },
    {
      "PickNo": "WHSE PICK-03610",
      "ItemNo": "ITEM SERIAL TEST",
      "VariantCode": "",
      "SerialNo": "2",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "LocationCode": "MAIN",
      "BinCode": "BACK",
      "UnitofMeasureCode": "EA",
      "LP": "LP-00023",
      "PriorityScore": 4.0,
      "QtyInLP": 1.0,
      "QtyToTake": 1.0,
      "QtyOrignalRequested": 3.0,
      "QtyRemaingRequested": 2.0,
      "NeedToSplit": true,
      "SufficientToFulfill": false
    },
    {
      "PickNo": "WHSE PICK-03610",
      "ItemNo": "ITEM SERIAL TEST",
      "VariantCode": "",
      "SerialNo": "4",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "LocationCode": "MAIN",
      "BinCode": "BACK",
      "UnitofMeasureCode": "EA",
      "LP": "LP-00023",
      "PriorityScore": 4.0,
      "QtyInLP": 1.0,
      "QtyToTake": 1.0,
      "QtyOrignalRequested": 3.0,
      "QtyRemaingRequested": 1.0,
      "NeedToSplit": true,
      "SufficientToFulfill": false
    },
    {
      "PickNo": "WHSE PICK-03610",
      "ItemNo": "D0AVESVTBLU00S",
      "VariantCode": "",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "LocationCode": "MAIN",
      "BinCode": "BACK",
      "UnitofMeasureCode": "EA",
      "LP": "LP-00023",
      "PriorityScore": 4.0,
      "QtyInLP": 5.0,
      "QtyToTake": 2.0,
      "QtyOrignalRequested": 2.0,
      "QtyRemaingRequested": 2.0,
      "NeedToSplit": true,
      "SufficientToFulfill": true
    }
  ]
}
```

#### **Response Fields**
- **PickNo**: Número del Warehouse Pick asociado (e.g., `"WHSE PICK-03610"`).
- **ItemNo**: Número del artículo en el LP (e.g., `"ITEM SERIAL TEST"`).
- **VariantCode**: Código de variante del artículo, si aplica.
- **SerialNo**: Número de serie del artículo, si aplica.
- **LotNo**: Número de lote del artículo, si aplica.
- **ExpirationDate**: Fecha de expiración del artículo en el LP, si aplica (e.g., `"2024-01-01"`).
- **LocationCode**: Código de la ubicación del almacén (e.g., `"MAIN"`).
- **BinCode**: Código del bin donde se encuentra el LP (e.g., `"BACK"`).
- **UnitofMeasureCode**: Unidad de medida del artículo (e.g., `"EA"`).
- **LP**: Número del License Plate (LP) seleccionado (e.g., `"LP-00023"`).
- **PriorityScore**: Puntaje de prioridad asignado a la selección del LP según las reglas de coincidencia.
- **QtyInLP**: Cantidad disponible en el LP (e.g., `1.0`).
- **QtyToTake**: Cantidad a tomar del LP para el Warehouse Pick (e.g., `1.0`).
- **QtyOrignalRequested**: Cantidad solicitada originalmente en el Warehouse Pick (e.g., `3.0`).
- **QtyRemaingRequested**: Cantidad que aún queda por satisfacer en el Warehouse Pick (e.g., `2.0`).
- **NeedToSplit**: Indica si es necesario dividir el LP para cumplir con la cantidad solicitada (e.g., `true`).
- **SufficientToFulfill**: Indica si el LP tiene suficiente cantidad para cumplir con la solicitud sin necesidad de splits (e.g., `false`).

#### **PriorityScore Calculation**
El **PriorityScore** se calcula según la combinación de los siguientes factores:

1. **ExactQuantities**: Indica si las cantidades en el LP coinciden exactamente con la cantidad solicitada.
2. **NoExtraItems**: Indica si el LP contiene ítems adicionales no solicitados.

La lógica del puntaje de prioridad es la siguiente:
- **PriorityScore = 1**: Coincidencia exacta sin ítems adicionales.
- **PriorityScore = 2**: Cantidad exacta con ítems adicionales.
- **PriorityScore = 3**: Cantidades suficientes o superiores sin ítems adicionales.
- **PriorityScore = 4**: Cantidades suficientes o superiores con ítems adicionales.
- **PriorityScore = 5**: Cantidades insuficientes sin ítems adicionales.
- **PriorityScore = 6**: Cantidades insuficientes con ítems adicionales.

#### **Consideraciones de Optimización**
- **Reducción de Divisiones (Splits)**: El sistema trata de minimizar los splits, priorizando los LPs que cumplan mejor con las cantidades solicitadas.
- **Escalabilidad**: El algoritmo está diseñado para manejar grandes volúmenes de datos de Warehouse Picks y LPs, optimizando la búsqueda y selección.
- **Compatibilidad con FEFO**: A futuro, el sistema puede considerar un enfoque **FEFO** (First Expired, First Out), priorizando LPs con fechas de expiración más próximas.

#### **Summary**
El método `GetAllOptimalLPSelections` proporciona una selección optimizada de License Plates basada en reglas de prioridad que consideran la coincidencia de cantidades