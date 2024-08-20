### **Pruebas Unitarias - Escenario Base Modificado**

#### **Propósito**
El propósito de esta prueba es verificar el correcto funcionamiento del proceso de creación, autoasignación y almacenamiento de License Plates (LPs) en un Warehouse Receipt (WR). En este escenario, se probará la capacidad del sistema para manejar múltiples LPs en una sola línea de WR, asegurando que se generen correctamente los registros necesarios en las tablas correspondientes y que todos los movimientos y estados se actualicen de manera coherente.

#### **Preparación**

1. **Ir al Warehouse Receipt**
   - **Acción**: Accede al documento de Warehouse Receipt que se utilizará para la prueba.
   - **Verificación**: Asegúrate de que el Warehouse Receipt contiene líneas con ítems listos para ser recibidos y que el documento está en estado "abierto".

2. **Creación y Autoasignación de License Plates (LPs)**
   - **Propósito**: Validar la creación y autoasignación de múltiples LPs asociados a una línea de Warehouse Receipt.
   - **Acción**: Utiliza la API `CreateLPFromWarehouseReceiptLine` para crear y autoasignar LPs a los ítems en una línea específica del Warehouse Receipt según los siguientes parámetros:
     - **No**: El número del Warehouse Receipt para el que se deben crear los LPs (por ejemplo, "WHSE REC-0001").
     - **ItemNo**: El número de ítem asociado a la línea del Warehouse Receipt (por ejemplo, "ITEM-001").
     - **BinCode**: El código del bin donde se almacenarán los ítems (por ejemplo, "BIN-01").
     - **LineNo**: El número de línea del Warehouse Receipt (por ejemplo, 10000).
     - **UnitofMeasureCode**: El código de la unidad de medida para los ítems (por ejemplo, "PCS").
     - **TotalToReceive**: La cantidad total de ítems a recibir (por ejemplo, 100).
     - **NoofPackLP**: El número de LPs a crear (por ejemplo, 10).
     - **PackUnitUoM**: La unidad de medida del empaque (por ejemplo, "BOX").
   - **Verificación**: Confirma que se han creado los LPs con el estado inicial "Received" en la tabla de "PLU LP New Headers" y que los ítems han sido autoasignados correctamente a los LPs.

3. **Posteo del Warehouse Receipt**
   - **Propósito**: Verificar que el posteo del Warehouse Receipt actualiza correctamente el estado del LP y registra los movimientos necesarios.
   - **Acción**: Postea el Warehouse Receipt usando la API `PostWarehouseReceipt`.
   - **Verificación**: Confirma que el estado de los LPs ha cambiado a "Labeled" en la tabla de "PLU LP New Headers" y que se ha registrado un movimiento en la tabla de "PLU LP Movements" con el tipo "Receive".

4. **Verificación de Put Away**
   - **Propósito**: Asegurar que los LPs están listos para ser almacenados correctamente.
   - **Acción**: Abre el Put Away asociado al Warehouse Receipt.
   - **Verificación**: Confirma que los LPs ahora están listos para ser movidos a su ubicación de almacenamiento, y que el estado y bin de los LPs en "PLU LP New Headers" se ha actualizado correctamente a "Labeled".

5. **Validación de Put Away Lines**
   - **Propósito**: Verificar la congruencia de los datos en las líneas de Put Away.
   - **Acción**: Revisa las líneas de Put Away en el documento.
   - **Verificación**: Asegúrate de que todas las líneas coinciden en cuanto a la ubicación de almacenamiento (bin) y que no existen inconsistencias en los datos.

6. **Registro del Put Away**
   - **Propósito**: Validar el proceso de almacenamiento final de los LPs.
   - **Acción**: Registra el Put Away usando la API `Post_WarehousePutAway`.
   - **Verificación**: Verifica que el estado de los LPs ha cambiado a "Stored" y que se han registrado dos movimientos en la tabla de "PLU LP Movements" (uno que refleja la salida del bin de recepción y otro que refleja la entrada en el bin de almacenamiento).

7. **Verificación Final**
   - **Propósito**: Asegurar la correcta finalización del proceso y la integridad de los datos.
   - **Acción**: Realiza una revisión completa de los LPs en la tabla de "PLU LP New Headers".
   - **Verificación**: Confirma que los LPs están en estado "Stored" y que todos los movimientos en la tabla "PLU LP Movements" están correctamente registrados, sin inconsistencias.

### **Conclusión**
Este plan de pruebas asegura una cobertura exhaustiva del proceso de creación, autoasignación, posteo y almacenamiento de LPs en un Warehouse Receipt. Implementar estas pruebas ayudará a identificar problemas antes de que el sistema sea desplegado en un entorno de producción, garantizando la fiabilidad y exactitud del sistema en la gestión de inventarios.

----------------
### **Pruebas Unitarias - Escenario con Creación de LPs Vacíos**

#### **Propósito**
El objetivo de esta prueba es verificar el proceso de creación de License Plates (LPs) vacíos mediante la API `CreateEmptyLPFromWarehouseReceipt`, seguido de la asignación de ítems a estos LPs usando la API `AssignItemToLPFromWarehouseReceipt`. Esta prueba asegurará que los LPs vacíos se creen y que los ítems se asignen correctamente, manteniendo la integridad de los datos en el sistema.

#### **Preparación**

1. **Ir al Warehouse Receipt**
   - **Acción**: Accede al documento de Warehouse Receipt que se utilizará para la prueba.
   - **Verificación**: Asegúrate de que el Warehouse Receipt contiene líneas con ítems listos para ser recibidos y que el documento está en estado "abierto".

#### **Creación de LPs Vacíos**

2. **Creación de License Plates Vacíos**
   - **Propósito**: Validar la creación de LPs vacíos asociados a un Warehouse Receipt.
   - **Acción**: Utiliza la API `CreateEmptyLPFromWarehouseReceipt` para crear LPs vacíos asociados al Warehouse Receipt. Los parámetros son:
     - **WarehouseReceiptNo**: El número del Warehouse Receipt para el que se deben crear los LPs vacíos (por ejemplo, "WHSE REC-0001").
   - **Verificación**: Confirma que los LPs se han creado con el estado inicial "Received" en la tabla de "PLU LP New Headers" y que no contienen ítems asignados inicialmente.

#### **Asignación de Ítems a LPs Vacíos**

3. **Asignación de Ítems a los LPs Vacíos**
   - **Propósito**: Verificar que los ítems puedan ser asignados correctamente a los LPs vacíos creados en el paso anterior.
   - **Acción**: Utiliza la API `AssignItemToLPFromWarehouseReceipt` para asignar ítems a los LPs vacíos. Los parámetros son:
     - **LPDocumentNo**: El número del LP vacío creado en el paso anterior.
     - **ItemNo**: El número del ítem a asignar (por ejemplo, "ITEM-001").
     - **VariantCode**: El código de variante del ítem (si aplica).
     - **QtyToReceive**: La cantidad de ítems a recibir y asignar al LP.
     - **UnitofMeasureCode**: El código de la unidad de medida para los ítems.
     - **WarehouseReceiptNo**: El número del Warehouse Receipt.
     - **WarehouseReceiptLineNo**: El número de línea específico del Warehouse Receipt asociado al ítem.
   - **Verificación**: Revisa que la cantidad del ítem se ha actualizado correctamente en la tabla de "PLU LP New Lines" y que el estado del LP permanece en "Received".

4. **Asignación de un Segundo Ítem al LP**
   - **Propósito**: Validar que múltiples ítems puedan ser asignados a un solo LP vacío.
   - **Acción**: Repite el paso 3, esta vez asignando un segundo ítem o variante al mismo LP.
   - **Verificación**: Confirma que ambos ítems están correctamente asociados al LP y que no se ha generado ningún error en la asignación.

#### **Posteo del Warehouse Receipt**

5. **Posteo del Warehouse Receipt**
   - **Propósito**: Verificar que el posteo del Warehouse Receipt actualiza correctamente el estado del LP y registra los movimientos necesarios.
   - **Acción**: Postea el Warehouse Receipt usando la API `PostWarehouseReceipt`.
   - **Verificación**: Confirma que el estado de los LPs ha cambiado a "Labeled" en la tabla de "PLU LP New Headers" y que se ha registrado un movimiento en la tabla de "PLU LP Movements" con el tipo "Receive".

#### **Verificación de Put Away**

6. **Verificación de Put Away**
   - **Propósito**: Asegurar que los LPs están listos para ser almacenados correctamente.
   - **Acción**: Abre el Put Away asociado al Warehouse Receipt.
   - **Verificación**: Confirma que los LPs ahora están listos para ser movidos a su ubicación de almacenamiento, y que el estado y bin de los LPs en "PLU LP New Headers" se ha actualizado correctamente a "Labeled".

7. **Validación de Put Away Lines**
   - **Propósito**: Verificar la congruencia de los datos en las líneas de Put Away.
   - **Acción**: Revisa las líneas de Put Away en el documento.
   - **Verificación**: Asegúrate de que todas las líneas coinciden en cuanto a la ubicación de almacenamiento (bin) y que no existen inconsistencias en los datos.

#### **Registro del Put Away**

8. **Registro del Put Away**
   - **Propósito**: Validar el proceso de almacenamiento final de los LPs.
   - **Acción**: Registra el Put Away usando la API `Post_WarehousePutAway`.
   - **Verificación**: Verifica que el estado de los LPs ha cambiado a "Stored" y que se han registrado dos movimientos en la tabla de "PLU LP Movements" (uno que refleja la salida del bin de recepción y otro que refleja la entrada en el bin de almacenamiento).

#### **Verificación Final**

9. **Verificación Final**
   - **Propósito**: Asegurar la correcta finalización del proceso y la integridad de los datos.
   - **Acción**: Realiza una revisión completa de los LPs en la tabla de "PLU LP New Headers".
   - **Verificación**: Confirma que los LPs están en estado "Stored" y que todos los movimientos en la tabla "PLU LP Movements" están correctamente registrados, sin inconsistencias.

### **Variantes y Escenarios Adicionales**

- **Escenario con Múltiples LPs Vacíos**
  - Realiza el mismo flujo pero creando varios LPs vacíos y asignando ítems a cada uno de ellos. Verifica que todos los LPs se manejen correctamente en cada paso del proceso.

- **Escenario con LP Parent y Múltiples Hijos**
  - Crea un LP Parent vacío y asigna varios LPs hijos (también vacíos) a él antes de asignar los ítems. Asegúrate de que las relaciones parent-child se mantengan correctamente y que los movimientos asociados se registren sin errores.

### **Conclusión**
Este plan de pruebas asegura una cobertura detallada del proceso de creación de LPs vacíos, su asignación y el posterior almacenamiento en el Warehouse Receipt. Implementar estas pruebas ayudará a identificar problemas antes de que el sistema sea desplegado en un entorno de producción, garantizando la fiabilidad y exactitud del sistema en la gestión de inventarios.