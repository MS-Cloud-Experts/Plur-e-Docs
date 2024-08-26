### API Documentation: AdjustLPQuantities

#### **Overview**
El método `AdjustLPQuantities` permite ajustar las cantidades en las líneas de un License Plate (LP) existente en un almacén. Este ajuste puede ser positivo (incremento) o negativo (decremento). Si el ajuste reduce la cantidad de una línea a cero, la línea se elimina. Si todas las líneas de un LP se eliminan, el LP se marca como "Voided". Además, se genera un Warehouse Item Journal para reflejar estos cambios en el inventario de Business Central, y se registran los movimientos en la tabla de LP Movements para mantener la trazabilidad.

#### **Request Structure**
```json
{
  "ProcessMethod": "AdjustLPQuantities",
  "Parameters": [
    {
      "LPDocumentNo": "LP-00113",
      "ItemNo": "K3PDBHNDL000XXX",
      "VariantCode": "",
      "AdjustQty": 3,
      "TrackingInfo": []
    },
    {
      "LPDocumentNo": "LP-00113",
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "AdjustQty": -1,
      "TrackingInfo": [
        {
          "LineNo": 20000,
          "SerialNo": "1SN0011111",
          "LotNo": "",
          "ExpirationDate": "",
          "Qty": 1
        }
      ]
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
  - **AdjustQty**: La cantidad a ajustar (positiva para incrementar, negativa para decrementar) (e.g., `-10`).
  - **TrackingInfo**: Información de rastreo, si aplica, que incluye las líneas específicas del LP a ajustar.
    - **LineNo**: El número de la línea en el LP que se va a ajustar (e.g., `10000`).
    - **SerialNo**: El número de serie del artículo, si aplica (e.g., `"SN001"`).
    - **LotNo**: El número de lote del artículo, si aplica (e.g., `"LOT001"`).
    - **ExpirationDate**: La fecha de expiración del artículo, si aplica (e.g., `"2024-12-31"`).
    - **Qty**: La cantidad específica relacionada al número de serie o lote que se va a ajustar (e.g., `5`).

#### **Example Request**
```json
{
  "ProcessMethod": "AdjustLPQuantities",
  "Parameters": [
    {
      "LPDocumentNo": "LP001",
      "ItemNo": "ITEM001",
      "VariantCode": "",
      "AdjustQty": -10,
      "TrackingInfo": [
        {
          "LineNo": 10000,
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
      "AdjustQty": 15,
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
El método `AdjustLPQuantities` permite ajustar cantidades en las líneas de License Plates existentes, tanto en incrementos como en decrementos. El API asegura que los ajustes se reflejen correctamente en el inventario mediante la creación de un Warehouse Item Journal y la actualización de los registros de movimientos de LP. Si un LP queda sin líneas, se marca automáticamente como "Voided".

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

### **Consideraciones Adicionales**
- **Uso de `TrackingInfo`**: El array `TrackingInfo` solo se utiliza cuando se necesitan introducir o ajustar seriales o lotes específicos. Si se va a ajustar una línea ya existente sin seriales o lotes, no es necesario incluir este array, lo que simplifica la operación.
- **Estado del LP**: Después de realizar todos los ajustes, el estado del LP se actualiza a "Processing". Una vez que el Warehouse Journal se postea exitosamente, el estado cambia a "Storage", asegurando la integridad y el seguimiento de los LPs dentro del sistema.