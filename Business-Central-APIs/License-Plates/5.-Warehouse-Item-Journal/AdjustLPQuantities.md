### Diseño del API: AdjustLPQuantities

#### 1. **Parámetros del API**
   - **ProcessMethod**: `"AdjustLPQuantities"`
   - **Parameters**: Un array de objetos que representan los ajustes que se desean realizar en las líneas de LPs existentes.
     - **LPDocumentNo**: Número de documento del LP a ajustar.
     - **ItemNo**: Número del artículo asociado con el LP.
     - **VariantCode**: Código de variante del artículo (si aplica).
     - **LocationCode**: Código de la ubicación del almacén.
     - **BinCode**: Código del bin donde se encuentra el LP.
     - **AdjustQty**: Cantidad a ajustar (positiva para incrementar, negativa para decrementar).
     - **UnitOfMeasureCode**: Código de la unidad de medida.
     - **TrackingInfo**: Información de rastreo, si aplica (SerialNo, LotNo, ExpirationDate, Qty).

#### 2. **Proceso Interno**
   - **Validación**: Validar que el LP y sus líneas existan, y que el ajuste sea coherente (por ejemplo, no permitir que el ajuste resulte en cantidades negativas no válidas).
   - **Aplicar Ajustes**: 
     - Si la cantidad ajustada es positiva, se incrementa la cantidad en la línea del LP.
     - Si la cantidad ajustada es negativa, se decrementa la cantidad en la línea del LP.
     - Si una línea de LP llega a cero, se elimina.
     - Si todas las líneas de un LP se eliminan, el LP se coloca en estado "Voided".
   - **Generación de Journal**: Generar un Warehouse Item Journal que refleje el ajuste de inventario en Business Central.
   - **Registro en Movimientos de LP**: Registrar el ajuste en la tabla de LP Movements para asegurar la trazabilidad.

#### 3. **Posteo**
   - Durante el posteo del Warehouse Item Journal, verificar que los cambios se reflejen correctamente en los registros de LP y en el inventario.
   - Asegurar que se generen los movimientos correspondientes en la tabla de LP Movements.

### Proceso de Desarrollo
1. **Desarrollo Iterativo**:
   - **Primera fase**: Implementar el ajuste básico de cantidades en LPs (sin rastreo, solo el ajuste directo).
   - **Segunda fase**: Añadir soporte para información de rastreo (SerialNo, LotNo, etc.).
   - **Tercera fase**: Implementar la lógica para eliminar líneas y LPs, y marcar el LP como "Voided" si todas las líneas son eliminadas.
   - **Cuarta fase**: Implementar la generación del Warehouse Item Journal y los movimientos de LP.

2. **Pruebas Unitarias**:
   - **Ajustes Positivos**: Verificar que al incrementar la cantidad en una línea de LP, el cambio se refleje correctamente en el inventario y en los movimientos.
   - **Ajustes Negativos**: Verificar que al decrementar la cantidad en una línea de LP, el cambio se refleje correctamente y que las líneas o LPs se eliminen cuando corresponda.
   - **Manejo de Errores**: Asegurar que se manejen adecuadamente casos como intentar decrementar una cantidad mayor a la disponible o manejar cantidades negativas no válidas.

3. **Validaciones Finales**:
   - Revisar que todo el proceso sea trazable y auditable, garantizando la integridad del inventario y de los registros de LP.
