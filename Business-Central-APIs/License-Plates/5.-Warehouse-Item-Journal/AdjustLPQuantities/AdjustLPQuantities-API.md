### API Documentation: AdjustLPQuantities

#### **Overview**
El método `AdjustLPQuantities` permite ajustar las cantidades en las líneas de un License Plate (LP) existente en un almacén. Este ajuste puede ser positivo (incremento) o negativo (decremento). Si el ajuste reduce la cantidad de una línea a cero, la línea se elimina. Si todas las líneas de un LP se eliminan, el LP se marca como "Voided". Adicionalmente, se genera un Warehouse Item Journal para reflejar estos cambios en el inventario de Business Central, y se registran los movimientos en la tabla de LP Movements.

#### **Request Structure**
```json
{
  "ProcessMethod": "AdjustLPQuantities",
  "Parameters": [
    {
      "LPDocumentNo": "LP001",
      "ItemNo": "ITEM001",
      "VariantCode": "",
      "LocationCode": "MAIN",
      "BinCode": "BIN-01",
      "AdjustQty": -10,
      "UnitOfMeasureCode": "EA",
      "TrackingInfo": [
        {
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Qty": 5
        }
      ]
    },
    {
      "LPDocumentNo": "LP002",
      "ItemNo": "ITEM002",
      "VariantCode": "",
      "LocationCode": "MAIN",
      "BinCode": "BIN-02",
      "AdjustQty": 15,
      "UnitOfMeasureCode": "EA",
      "TrackingInfo": []
    }
  ]
}
```

#### **Parameters**
- **ProcessMethod**: Indica el método a invocar, en este caso `"AdjustLPQuantities"`.
- **Parameters**: Un array de objetos que describen los ajustes a realizar en los LPs.
  - **LPDocumentNo**: El número de documento del LP a ajustar (e.g., `"LP001"`).
  - **ItemNo**: El número del artículo asociado al LP (e.g., `"ITEM001"`).
  - **VariantCode**: El código de variante del artículo, si aplica (e.g., `""`).
  - **LocationCode**: El código de la ubicación del almacén (e.g., `"MAIN"`).
  - **BinCode**: El código del bin donde se encuentra el LP (e.g., `"BIN-01"`).
  - **AdjustQty**: La cantidad a ajustar (positiva para incrementar, negativa para decrementar) (e.g., `-10`).
  - **UnitOfMeasureCode**: El código de la unidad de medida (e.g., `"EA"`).
  - **TrackingInfo**: Información de rastreo, si aplica.
    - **SerialNo**: El número de serie del artículo, si aplica (e.g., `"SN001"`).
    - **LotNo**: El número de lote del artículo, si aplica (e.g., `"LOT001"`).
    - **ExpirationDate**: La fecha de expiración del artículo, si aplica (e.g., `"2024-12-31"`).
    - **Qty**: La cantidad específica relacionada al número de serie o lote (e.g., `5`).

#### **Example Request**
```json
{
  "ProcessMethod": "AdjustLPQuantities",
  "Parameters": [
    {
      "LPDocumentNo": "LP001",
      "ItemNo": "ITEM001",
      "VariantCode": "",
      "LocationCode": "MAIN",
      "BinCode": "BIN-01",
      "AdjustQty": -10,
      "UnitOfMeasureCode": "EA",
      "TrackingInfo": [
        {
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Qty": 5
        }
      ]
    },
    {
      "LPDocumentNo": "LP002",
      "ItemNo": "ITEM002",
      "VariantCode": "",
      "LocationCode": "MAIN",
      "BinCode": "BIN-02",
      "AdjustQty": 15,
      "UnitOfMeasureCode": "EA",
      "TrackingInfo": []
    }
  ]
}
```

#### **Example Response**
```json
{
  "AdjustedLPs": [
    {
      "LPDocumentNo": "LP001",
      "AdjustedQty": -10,
      "RemainingLines": [
        {
          "ItemNo": "ITEM001",
          "VariantCode": "",
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "Quantity": 0
        }
      ]
    },
    {
      "LPDocumentNo": "LP002",
      "AdjustedQty": 15,
      "RemainingLines": [
        {
          "ItemNo": "ITEM002",
          "VariantCode": "",
          "SerialNo": "",
          "LotNo": "",
          "Quantity": 15
        }
      ]
    }
  ],
  "VoidedLPs": [
    {
      "LPDocumentNo": "LP001",
      "Message": "The LP was voided as it has no remaining lines."
    }
  ]
}
```

#### **Explanation**
- **AdjustedLPs**: Un array que muestra los LPs que han sido ajustados, con detalles sobre las líneas restantes después del ajuste.
- **VoidedLPs**: Un array que muestra los LPs que fueron marcados como "Voided" debido a que todas sus líneas fueron eliminadas tras los ajustes.

#### **Summary**
El método `AdjustLPQuantities` permite ajustar cantidades en las líneas de License Plates existentes, tanto en incrementos como en decrementos. El API se asegura de que los ajustes se reflejen correctamente en el inventario mediante la creación de un Warehouse Item Journal y la actualización de los registros de movimientos de LP. Si un LP queda sin líneas, se marca automáticamente como "Voided".

### Lógica de Implementación
1. **Validaciones Iniciales**: 
   - Verificar que el LP exista y que las cantidades a ajustar sean válidas.
   - Asegurar que los LPs y sus líneas están en un estado que permita el ajuste.

2. **Aplicar Ajustes**:
   - Para incrementos, sumar la cantidad a la línea correspondiente del LP.
   - Para decrementos, restar la cantidad y eliminar la línea si la cantidad llega a cero.
   - Si todas las líneas de un LP son eliminadas, cambiar el estado del LP a "Voided".

3. **Posteo del Warehouse Journal**:
   - Crear y postear un Warehouse Item Journal para reflejar los ajustes realizados.
   - Registrar los movimientos en la tabla de LP Movements para mantener la trazabilidad.
