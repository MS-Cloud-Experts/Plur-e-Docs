### **Documento del Proceso de Creación y Gestión de License Plates (LP)**

## **1. Introducción**

El proceso de creación y gestión de License Plates (LPs) en Business Central es crucial para optimizar la operación y gestión de inventarios en almacenes de gran envergadura. Un LP, o **License Plate**, permite agrupar ítems o incluso otros LPs bajo un mismo identificador único, facilitando la administración de los flujos logísticos como la recepción, almacenamiento, movimientos y envíos. Este enfoque no solo mejora la eficiencia, sino que también asegura la trazabilidad y el control sobre el inventario.

## **2. Principios Fundamentales y Estructura del Sistema**

### **2.1 Concepto de LP como Entidad Única**

Un **License Plate (LP)** es un identificador único que agrupa ítems o incluso otros LPs, formando una unidad lógica dentro del inventario. Esto permite realizar operaciones masivas y coordinadas sobre un conjunto de productos como si fueran un solo ítem, simplificando la gestión operativa desde la recepción de mercancías hasta el despacho.

### **2.2 Estructura Jerárquica Multinivel**

Los LPs pueden organizarse en una **estructura jerárquica multinivel**, donde un LP padre puede contener uno o varios LPs hijos. Esta estructura es útil en escenarios donde se manipulan grandes contenedores, palets o cajas que incluyen diversos ítems o subgrupos de productos, permitiendo una gestión eficiente tanto del LP principal como de sus elementos subordinados.

### **2.3 Tabla LP Movements**

La tabla **LP Movements** es fundamental en la gestión de LPs. Registra todos los movimientos realizados sobre los LPs, incluyendo entradas y salidas de inventario, transferencias entre ubicaciones (bins) y cambios de estado. Esta tabla asegura la **trazabilidad completa** de cada LP, permitiendo auditorías y revisiones detalladas de los movimientos en el almacén.

## **3. Estados de License Plates (LP)**

Los LPs pasan por una serie de estados que reflejan las diferentes fases de su ciclo de vida dentro del almacén. Estos estados permiten gestionar adecuadamente los procesos operativos y garantizar un control sobre el inventario. Los principales estados de un LP son:

1. **Pre-Labeled**: El LP ha sido creado pero no ha sido asignado a un proceso logístico.
2. **Received**: El LP ha sido registrado durante la recepción de mercancía.
3. **Labeled**: El LP ha sido etiquetado y está listo para ser almacenado.
4. **Stored**: El LP ha sido ubicado en su espacio de almacenamiento en el almacén.
5. **Picked**: El LP ha sido seleccionado para un pedido o envío.
6. **Packed**: El LP ha sido empaquetado y está listo para su envío.
7. **Voided**: El LP ha sido anulado y no puede volver a ser utilizado.
8. **Blocked/Reserved**: El LP está bloqueado o reservado y no puede manipularse hasta que sea liberado.
9. **Processing**: El LP está en proceso de ser manipulado o preparado para un uso específico.
10. **Released**: El LP ha sido liberado de cualquier restricción y está listo para ser manipulado.
11. **Inspecting**: El LP está en proceso de inspección.
12. **Hold**: El LP está en estado de retención, posiblemente por una anomalía.
13. **Damaged**: El LP contiene ítems dañados y necesita tratamiento especial.
14. **Pending**: El LP está pendiente de una acción adicional, como un movimiento o ajuste.

## **4. Reglas de Integridad y Movimientos**

### **4.1 Integridad del Inventario**

Las cantidades totales de los ítems agrupados en los LPs deben coincidir con las cantidades físicas reales en el almacén. El sistema valida esta integridad continuamente, y cualquier discrepancia debe corregirse de inmediato para garantizar un control riguroso del inventario.

### **4.2 Restricciones de Capacidad**

Cada LP debe cumplir con las restricciones de capacidad de los bins en los que se almacenan, incluyendo consideraciones de peso, volumen y tipo de ítems. Estas restricciones garantizan que el almacén mantenga una estructura organizada y que los bins no se sobrecarguen.

### **4.3 Movimientos entre Bins**

Los LPs pueden moverse entre diferentes ubicaciones (bins) dentro del almacén para optimizar el espacio disponible o preparar los productos para su siguiente etapa en el proceso logístico. Cada movimiento se registra en la tabla **LP Movements**, asegurando que todas las operaciones estén correctamente documentadas.

### **4.4 Compatibilidad de Estados**

Solo los LPs en ciertos estados, como "Stored" o "Received", pueden ser unidos o movidos. Los LPs en estado "Blocked", "Hold" o "Damaged" no pueden ser manipulados hasta que se resuelva su situación, asegurando que no se interfiera con operaciones críticas.

## **5. Operaciones sobre License Plates (LP)**

### **5.1 Split (División) de LPs**

El proceso de **split** permite dividir un LP en varios LPs nuevos. Este proceso es útil cuando se necesita dividir grandes cantidades de productos para reubicarlos o distribuirlos de manera más eficiente. Por ejemplo, un palet con 100 unidades puede dividirse en dos LPs: uno con 60 y otro con 40 unidades.

### **5.2 Join (Unión) de LPs**

El proceso de **join** permite combinar varios LPs en uno solo, consolidando sus ítems. Este proceso es beneficioso cuando se desea optimizar el espacio en el almacén o agrupar productos dispersos en un solo LP para facilitar su manejo o envío.

### **5.3 Movimientos entre Bins**

Los LPs pueden moverse de un bin a otro dentro del almacén para mejorar la distribución del inventario o preparar los productos para su envío. Estos movimientos son gestionados y registrados automáticamente, asegurando que todos los cambios de ubicación sean documentados.

### **5.4 Proceso de Conteo Físico**

Durante el conteo físico de inventario, los LPs son fundamentales para consolidar las cantidades de productos y asegurar que las cantidades físicas coincidan con los registros en el sistema. Este proceso ayuda a identificar discrepancias y mantener un control constante sobre los niveles de inventario.

## **6. Procesos de Compras**

### **6.1 Recepción de Mercancías (Wshe Receive)**

En este proceso, las mercancías recibidas de proveedores son registradas en el sistema. Los LPs se crean o actualizan para reflejar los ítems recibidos, asegurando un registro preciso desde el inicio.

### **6.2 Almacenamiento (Wshe PutAway)**

Los ítems recibidos son ubicados en el almacén. Los LPs ayudan a agrupar los ítems para su movimiento eficiente hacia las ubicaciones designadas.

### **6.3 Registro de Almacenamiento (Wshe Registered PutAway)**

Se finaliza el proceso de almacenamiento, registrando en el sistema que los ítems han sido ubicados correctamente y actualizando el estado de los LPs a "Stored".

## **7. Procesos de Ventas**

### **7.1 Envíos de Almacén (Wshe Shipments)**

Se generan los envíos de almacén para preparar las órdenes de venta. Aquí se planifican las operaciones necesarias para cumplir con los pedidos de los clientes.

### **7.2 Preparación de Pedidos (Wshe Picks)**

La **preparación de pedidos (Picks)** es uno de los módulos más importantes de todo el proceso de ventas. En esta etapa, se seleccionan y asignan los ítems necesarios para cumplir con los pedidos, utilizando los LPs de manera óptima.

#### **7.2.1 Selección Óptima de LPs para Picking**

Se ha implementado una funcionalidad avanzada que permite determinar la **mejor selección de LPs** para satisfacer las órdenes de picking. Esta selección óptima es crucial para mejorar la eficiencia y precisión en el cumplimiento de pedidos.

##### **7.2.1.1 Selección Óptima de LPs**

El sistema utiliza algoritmos especializados para analizar la disponibilidad de LPs y seleccionar aquellos que mejor se ajustan a las necesidades del pick. Se consideran factores como las cantidades requeridas, fechas de caducidad y la composición de los LPs.

##### **7.2.1.2 Cálculo de Necesidades y Disponibilidad**

El sistema realiza un cálculo detallado que incluye:

- **Cantidades Totales Requeridas**: Basadas en las líneas de actividad del almacén para el pick.
- **Cantidades Asignadas**: Ítems que ya han sido asignados a LPs previamente.
- **Cantidades Restantes**: Diferencia entre lo requerido y lo asignado, indicando lo que aún falta por cubrir.

##### **7.2.1.3 Prioritización y Selección de LPs**

Se priorizan los LPs según criterios como:

- **Fecha de Caducidad (FEFO)**: Se seleccionan primero los LPs con fechas de caducidad más próximas.
- **Exactitud en Contenido**: Preferencia por LPs que contienen exactamente los ítems y cantidades requeridas, evitando ítems adicionales.
- **Eficiencia Operativa**: Se buscan LPs que puedan satisfacer múltiples requerimientos para minimizar movimientos y manipulaciones.

##### **7.2.1.4 Beneficios de la Selección Óptima**

- **Eficiencia Mejorada**: Reducción de tiempos en la preparación de pedidos.
- **Minimización de Errores**: Al seleccionar los LPs más adecuados, se reduce la posibilidad de errores en el picking.
- **Optimización de Recursos**: Uso más efectivo de los LPs disponibles, evitando sobreasignaciones o desperdicios.

#### **7.2.2 Gestión Avanzada de LPs en Órdenes de Picking**

Esta funcionalidad permite una administración detallada de los LPs asignados a las órdenes de picking, mejorando el control y la flexibilidad.

##### **7.2.2.1 Asignación de LPs a Órdenes de Picking**

- **Validación Automática**: El sistema verifica que los LPs seleccionados cumplen con los requisitos de los pedidos.
- **Actualización de Estados**: Los LPs cambian a estado "Picked" al ser asignados.
- **Registro Detallado**: Se documentan todas las asignaciones para mantener la trazabilidad.

##### **7.2.2.2 Remoción y Reasignación de LPs**

- **Flexibilidad en Operaciones**: Posibilidad de remover LPs asignados en caso de cambios en las órdenes.
- **Actualización Dinámica**: Los estados de los LPs y las cantidades en las órdenes se actualizan automáticamente.
- **Reasignación Eficiente**: Los LPs liberados pueden ser asignados a otras órdenes que los requieran.

##### **7.2.2.3 Monitoreo y Estado de Asignaciones**

- **Visualización en Tiempo Real**: Información actualizada sobre las asignaciones y necesidades pendientes.
- **Alertas y Notificaciones**: El sistema alerta sobre discrepancias o necesidades no cubiertas.
- **Informes y Análisis**: Generación de informes para mejorar la planificación y la toma de decisiones.

##### **7.2.2.4 Impacto en la Operación**

- **Productividad Aumentada**: Procesos más eficientes reducen tiempos y aumentan la capacidad operativa.
- **Satisfacción del Cliente**: Cumplimiento preciso y rápido de los pedidos mejora la experiencia del cliente.
- **Adaptabilidad**: La gestión flexible permite responder rápidamente a cambios en la demanda o en el inventario.

### **7.3 Registro de Preparación (Wshe Registered Picks)**

Una vez completada la preparación de los pedidos, se registra en el sistema, actualizando los estados de los LPs y asegurando que el inventario refleje con precisión las salidas de productos.

## **8. Ventas y Proceso de Assemblies**

Para los procesos de ventas, se requiere un proceso de **Assemblies** para construir **Kits** de productos. Estos **Kits** permiten combinar diferentes ítems bajo una sola oferta comercial. Además, el sistema está diseñado para buscar automáticamente sustitutos cuando alguno de los productos que componen el Kit no está disponible al momento de la venta, asegurando que el cliente reciba el producto sin interrupciones en el proceso logístico.

### **8.1 Ventajas del Proceso de Assemblies**

- **Automatización de Sustituciones**: Si uno de los componentes del Kit no está disponible, el sistema busca automáticamente sustitutos viables.
- **Optimización de Inventario**: Permite agrupar productos disponibles y gestionar de manera eficiente la creación de Kits para ventas.
- **Flexibilidad en la Operación**: Facilita la personalización de los Kits de acuerdo con la disponibilidad del inventario.

## **9. Optimización y Control**

### **9.1 Trazabilidad Completa**

Cada movimiento, cambio de estado o ajuste de los LPs es registrado, proporcionando una trazabilidad completa de cada ítem. Esto es clave para auditorías y control de inventarios, asegurando que se pueda rastrear cualquier producto en todo momento.

### **9.2 Escalabilidad**

El sistema de LPs está diseñado para escalar según las necesidades del almacén. Desde pequeñas operaciones hasta grandes volúmenes de productos, la flexibilidad de los LPs permite gestionar eficazmente el inventario sin importar la complejidad de los procesos.

### **9.3 Reglas de Validación**

El sistema incorpora reglas de validación estrictas para asegurar que todas las operaciones sobre los LPs cumplan con los requisitos de integridad del inventario, capacidad del bin y compatibilidad de estados. Cualquier discrepancia o problema se identifica automáticamente, permitiendo una corrección rápida.

## **10. Resumen**

La integración de funcionalidades avanzadas para la **selección óptima de LPs** y la **gestión eficiente de asignaciones en órdenes de picking** dentro del módulo de **Wshe Picks** mejora significativamente la operación logística en el almacén. Estas herramientas permiten:

- **Reducción de Costos**: Al optimizar la selección y uso de LPs, se minimizan los recursos necesarios.
- **Incremento en la Productividad**: Procesos más eficientes reducen tiempos y aumentan la capacidad operativa.
- **Mayor Satisfacción del Cliente**: Al cumplir con los pedidos de manera precisa y rápida, se mejora la experiencia del cliente final.
- **Adaptabilidad**: La flexibilidad en la gestión de LPs y asignaciones permite adaptarse a fluctuaciones en la demanda y cambios en el inventario.

La conceptualización y desarrollo de estas funcionalidades reflejan un compromiso con la **excelencia operacional** y la **innovación** en la gestión de inventarios y operaciones logísticas.