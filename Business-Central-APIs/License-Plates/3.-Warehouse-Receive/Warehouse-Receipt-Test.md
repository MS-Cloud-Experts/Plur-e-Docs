### **Pruebas Unitarias - Escenario Base Modificado**

#### **Propósito**
El propósito de esta prueba es verificar el correcto funcionamiento del proceso de creación, asignación y almacenamiento de License Plates (LPs) en un Warehouse Receipt (WR). En este escenario, se probará la capacidad del sistema para manejar múltiples LPs en una sola línea de WR, asegurando que se generen correctamente los registros necesarios en las tablas correspondientes y que todos los movimientos y estados se actualicen de manera coherente.

#### **Preparación**

1. **Ir al Warehouse Receipt**
   - **Acción**: Accede al documento de Warehouse Receipt que se utilizará para la prueba.
   - **Verificación**: Asegúrate de que el Warehouse Receipt contiene líneas con ítems listos para ser recibidos y que el documento está en estado "abierto".

2. **Creación de License Plates (LPs)**
   - **Propósito**: Validar la creación de múltiples LPs asociados a una línea de Warehouse Receipt.
   - **Acción**: Utiliza la API `CreateLPFromWarehouseReceiptLine` para crear varios LPs según los siguientes parámetros:
     - **No**: El número del Warehouse Receipt para el que se deben crear los LPs (por ejemplo, "WHSE REC-0001").
     - **ItemNo**: El número de ítem asociado a la línea del Warehouse Receipt (por ejemplo, "ITEM-001").
     - **BinCode**: El código del bin donde se almacenarán los ítems (por ejemplo, "BIN-01").
     - **LineNo**: El número de línea del Warehouse Receipt (por ejemplo, 10000).
     - **UnitofMeasureCode**: El código de la unidad de medida para los ítems (por ejemplo, "PCS").
     - **TotalToReceive**: La cantidad total de ítems a recibir (por ejemplo, 100).
     - **NoofPackLP**: El número de LPs a crear (por ejemplo, 10).
     - **PackUnitUoM**: La unidad de medida del empaque (por ejemplo, "BOX").
   - **Verificación**: Confirma que se han creado los LPs con el estado inicial "Received" en la tabla de "PLU LP New Headers".

3. **Asignación de un ítem a un LP**
   - **Propósito**: Verificar que un ítem puede ser correctamente asignado a un LP recién creado.
   - **Acción**: Selecciona un ítem del Warehouse Receipt y asígnalo a uno de los LPs creados usando la API `AssignItemToLPFromWarehouseReceipt`.
   - **Verificación**: Revisa que la cantidad del ítem se haya actualizado correctamente en la tabla de "PLU LP New Lines" y que el estado del LP permanezca en "Received".

4. **Asignación de un segundo ítem al mismo LP**
   - **Propósito**: Validar que se pueden asignar múltiples ítems o variantes al mismo LP sin problemas.
   - **Acción**: Repite el paso anterior, esta vez asignando un segundo ítem o variante al mismo LP.
   - **Verificación**: Confirma que ambos ítems están correctamente asociados al LP y que no se ha generado ningún error en la asignación.

5. **Posteo del Warehouse Receipt**
   - **Propósito**: Verificar que el posteo del Warehouse Receipt actualiza correctamente el estado del LP y registra los movimientos necesarios.
   - **Acción**: Postea el Warehouse Receipt usando la API `PostWarehouseReceipt`.
   - **Verificación**: Confirma que el estado del LP ha cambiado a "Labeled" en la tabla de "PLU LP New Headers" y que se ha registrado un movimiento en la tabla de "PLU LP Movements" con el tipo "Receive".

6. **Verificación de Put Away**
   - **Propósito**: Asegurar que el LP está listo para ser almacenado correctamente.
   - **Acción**: Abre el Put Away asociado al Warehouse Receipt.
   - **Verificación**: Confirma que el LP ahora está listo para ser movido a su ubicación de almacenamiento, y que el estado y bin del LP en "PLU LP New Headers" se han actualizado correctamente a "Labeled".

7. **Validación de Put Away Lines**
   - **Propósito**: Verificar la congruencia de los datos en las líneas de Put Away.
   - **Acción**: Revisa las líneas de Put Away en el documento.
   - **Verificación**: Asegúrate de que todas las líneas coinciden en cuanto a la ubicación de almacenamiento (bin) y que no existen inconsistencias en los datos.

8. **Registro del Put Away**
   - **Propósito**: Validar el proceso de almacenamiento final del LP.
   - **Acción**: Registra el Put Away usando la API `Post_WarehousePutAway`.
   - **Verificación**: Verifica que el estado del LP ha cambiado a "Stored" y que se han registrado dos movimientos en la tabla de "PLU LP Movements" (uno que refleja la salida del bin de recepción y otro que refleja la entrada en el bin de almacenamiento).

9. **Verificación Final**
   - **Propósito**: Asegurar la correcta finalización del proceso y la integridad de los datos.
   - **Acción**: Realiza una revisión completa del LP en la tabla de "PLU LP New Headers".
   - **Verificación**: Confirma que el LP está en estado "Stored" y que todos los movimientos en la tabla "PLU LP Movements" están correctamente registrados, sin inconsistencias.

### **Variantes y Escenarios Adicionales**

- **Escenario con Múltiples LPs**
  - Realiza el mismo flujo pero con varios LPs creados en una sola línea del Warehouse Receipt. Verifica que todos los LPs se manejen correctamente en cada paso del proceso.

- **Escenario con LP Parent y Múltiples Hijos**
  - Crea un LP Parent y asigna varios LPs hijos a él. Asegúrate de que las relaciones parent-child se mantengan correctamente y que los movimientos asociados se registren sin errores.

### **Conclusión**
Este plan de pruebas asegura una cobertura exhaustiva del proceso de creación, asignación, posteo y almacenamiento de LPs en un Warehouse Receipt. Implementar estas pruebas ayudará a identificar problemas antes de que el sistema sea desplegado en un entorno de producción, garantizando la fiabilidad y exactitud del sistema en la gestión de inventarios.