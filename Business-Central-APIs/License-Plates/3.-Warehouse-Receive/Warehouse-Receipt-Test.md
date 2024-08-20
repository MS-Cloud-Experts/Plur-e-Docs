### **Plan de Pruebas Humanas para el Proceso de Warehouse Receipt y Put Away en License Plates (LPs)**

#### **Objetivo General**
Validar que el proceso de creación, asignación y almacenamiento de License Plates (LPs) a través de un Warehouse Receipt (WR) funcione correctamente, asegurando que los LPs se actualicen adecuadamente en el sistema y que todos los movimientos asociados se registren correctamente en la tabla de PLU LP Movements.

#### **Pruebas Unitarias - Escenario Base**

1. **Preparación**
   - **Ir al Warehouse Receipt**: Accede al documento de Warehouse Receipt que se utilizará para la prueba.
   - **Verificación Previa**: Asegúrate de que el Warehouse Receipt contiene líneas con ítems listos para ser recibidos y que el documento está en estado "abierto".

2. **Creación de un License Plate (LP)**
   - **Acción**: Utiliza la API `CreateLPFromWarehouseReceiptLine` para crear un LP asociado a una línea del Warehouse Receipt.
   - **Verificación**: Confirma que el LP se ha creado con el estado inicial "Received" en la tabla de "PLU LP New Headers".

3. **Asignación de un ítem al LP**
   - **Acción**: Selecciona un ítem del Warehouse Receipt y asígnalo al LP creado usando la API `AssignItemToLPFromWarehouseReceipt`.
   - **Verificación**: Revisa que la cantidad del ítem se ha actualizado correctamente en la tabla de "PLU LP New Lines" y que el estado del LP permanece en "Received".

4. **Asignación de un segundo ítem al LP**
   - **Acción**: Repite el paso 3, esta vez asignando un segundo ítem o variante al mismo LP.
   - **Verificación**: Confirma que ambos ítems están correctamente asociados al LP y que no se ha generado ningún error en la asignación.

5. **Posteo del Warehouse Receipt**
   - **Acción**: Postea el Warehouse Receipt usando la API `PostWarehouseReceipt`.
   - **Verificación**: Confirma que el estado del LP ha cambiado a "Labeled" en la tabla de "PLU LP New Headers" y que se ha registrado un movimiento en la tabla de "PLU LP Movements" con el tipo "Receive".

6. **Verificación de Put Away**
   - **Acción**: Abre el Put Away asociado al Warehouse Receipt.
   - **Verificación**: Confirma que el LP ahora está listo para ser movido a su ubicación de almacenamiento, y que el estado y bin del LP en "PLU LP New Headers" se ha actualizado correctamente a "Labeled".

7. **Validación de Put Away Lines**
   - **Acción**: Revisa las líneas de Put Away en el documento.
   - **Verificación**: Asegúrate de que todas las líneas coinciden en cuanto a la ubicación de almacenamiento (bin) y que no existen inconsistencias en los datos.

8. **Registro del Put Away**
   - **Acción**: Registra el Put Away usando la API `Post_WarehousePutAway`.
   - **Verificación**: Verifica que el estado del LP ha cambiado a "Stored" y que se han registrado dos movimientos en la tabla de "PLU LP Movements" (uno que refleja la salida del bin de recepción y otro que refleja la entrada en el bin de almacenamiento).

9. **Verificación Final**
   - **Acción**: Realiza una revisión completa del LP en la tabla de "PLU LP New Headers".
   - **Verificación**: Confirma que el LP está en estado "Stored" y que todos los movimientos en la tabla "PLU LP Movements" están correctamente registrados, sin inconsistencias.