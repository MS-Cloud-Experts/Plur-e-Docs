### **Documento del Proceso de Creación y Gestión de License Plates (LP)**

## **1. Introducción**

Este documento detalla el proceso de creación y gestión de License Plates (LPs) en Business Central. Los LPs son esenciales para la administración eficiente de inventarios y garantizan una trazabilidad completa dentro de los almacenes. Este enfoque permite gestionar grandes volúmenes de inventario de manera estructurada, eficiente y escalable.

## **2. Principios Fundamentales y Estructura del Sistema**

### **2.1 Concepto de LP como Entidad Única**
Un License Plate (LP) es un identificador único que agrupa ítems o incluso otros LPs bajo un mismo número, facilitando la gestión del inventario. Un LP permite tratar un grupo de ítems como una sola entidad lógica, simplificando operaciones clave como la recepción, almacenamiento y envío de productos.

### **2.2 Estructura Jerárquica Multinivel**
Los LPs en Business Central pueden organizarse en una jerarquía multinivel. Un LP padre puede contener múltiples LPs hijos, formando una relación `parent-child`. Esto es útil para manejar grandes contenedores, palets o cajas que requieren movimientos coordinados y procesos logísticos complejos.

### **2.3 Tabla LP Movements**
Todos los movimientos relacionados con los LPs, como entradas y salidas de inventario, transferencias entre ubicaciones y cambios de estado, se registran en la tabla **LP Movements**. Esta tabla proporciona una trazabilidad completa de cada LP, asegurando la integridad de los datos y facilitando auditorías y revisiones.

## **3. Estados de License Plates (LP)**

Los LPs atraviesan varios estados a lo largo de su ciclo de vida, cada uno reflejando una etapa específica dentro del almacén. Estos estados incluyen:

1. **Pre-Labeled**: Estado inicial, el LP ha sido creado pero aún no asignado a un proceso.
2. **Received**: El LP ha sido registrado durante la recepción de mercancías.
3. **Labeled**: El LP está etiquetado y listo para almacenamiento.
4. **Stored**: El LP ha sido colocado en su ubicación final de almacenamiento.
5. **Picked**: El LP ha sido seleccionado para un pedido o envío.
6. **Packed**: El LP está empaquetado y listo para su despacho.
7. **Voided**: El LP ha sido anulado y no puede reutilizarse.
8. **Blocked/Reserved**: El LP está bloqueado o reservado para uso futuro.
9. **Process**: Estado que indica que el LP está en proceso de ser manipulado en alguna operación.

## **4. Reglas de Integridad y Movimientos**

### **4.1 Integridad del Inventario**
Es fundamental que las cantidades reflejadas en los LPs coincidan con las cantidades físicas reales en el almacén. Cualquier inconsistencia debe corregirse automáticamente durante el proceso de validación.

### **4.2 Restricciones de Capacidad**
Los LPs deben cumplir con las restricciones de capacidad y tipo de ítems del bin donde se almacenan. Esto asegura que no se sobrepase el límite de peso o volumen permitido.

### **4.3 Movimientos de LPs**
Todos los movimientos, tanto de LPs completos como de ítems individuales dentro de un LP, son registrados en la tabla "LP Movements" para mantener la trazabilidad. Esto incluye movimientos entre bins, cambios de estado y cualquier ajuste de inventario.

### **4.4 Compatibilidad de Estados**
Solo los LPs en estados compatibles, como "Stored" o "Received", pueden ser manipulados o unidos. LPs en estados como "Blocked" o "Reserved" deben ser liberados antes de cualquier operación adicional.

## **5. Operaciones sobre License Plates (LP)**

### **5.1 Split (División) de LPs**
Permite dividir un LP en varios LPs más pequeños. Por ejemplo, si un palet contiene 100 unidades, puedes dividirlo en dos LPs: uno con 60 y otro con 40 unidades para reubicar o distribuir los productos de manera eficiente.

### **5.2 Join (Unión) de LPs**
Combina varios LPs en uno solo para consolidar inventarios o facilitar el envío. Esta operación es útil cuando se necesitan agrupar productos dispersos en un solo contenedor o palet.

### **5.3 Movimientos entre Bins**
Los LPs pueden moverse entre diferentes ubicaciones dentro del almacén para optimizar el espacio o preparar productos para su siguiente etapa en el flujo logístico. Estos movimientos se registran automáticamente en la tabla "LP Movements".

### **5.4 Proceso de Conteo Físico**
El conteo físico de inventario permite ajustar las cantidades de los ítems asociados a un LP en base a la realidad física encontrada en el almacén. El registro de estos ajustes se realiza en el Warehouse Journal.

## **6. Procesos de Entrada y Salida**

### **6.1 Procesos de Entrada: Warehouse Receipt**
Durante la recepción de mercancías, los LPs son creados y asignados al estado "Received". Posteriormente, una vez que los productos se almacenan en su ubicación final, los LPs pasan al estado "Stored".

### **6.2 Procesos de Salida: Warehouse Shipments**
Al preparar productos para envío, los LPs seleccionados pasan al estado "Picked" y, después de empaquetarlos, cambian a "Packed". Finalmente, al ser despachados, los LPs se marcan como "Released".

### **6.3 Procesos de Entrada y Salida: Warehouse Item Journal**
El **Warehouse Item Journal** permite registrar entradas, salidas y ajustes de inventario a través de los LPs. Los LPs se crean o actualizan al registrar líneas en este journal, y todos los movimientos quedan reflejados en la tabla **LP Movements**.

## **7. API: Warehouse Item Journal – Conteo Físico de Inventario con LPs**

### **7.1 Introducción**
La API `Get_WarehouseInvPhysicalCount_LP` está diseñada para obtener el conteo físico de los ítems asociados con los LPs registrados en el Warehouse Journal. A través de esta API, se puede acceder a la jerarquía completa de los LPs y sus relaciones parent-child, facilitando un control detallado del inventario.

### **7.2 Conceptos Clave**

- **License Plates (LPs)**: Un LP es un identificador único asignado a un grupo de ítems en el almacén para su gestión y seguimiento.
- **Warehouse Journal**: Herramienta para registrar transacciones de inventario como ajustes o transferencias.
- **Jerarquía de LPs**: Los LPs pueden contener relaciones jerárquicas, permitiendo la creación de LPs padres que agrupan varios LPs hijos.

### **7.3 Procesos**

1. **Recepción de Parámetros**: La API recibe un JSON con los parámetros `JournalTemplateName`, `JournalBatchName`, y `LocationCode`, que definen el contexto del conteo físico.
   
2. **Filtrado de las Líneas del Warehouse Journal**: Se filtran las líneas del Warehouse Journal basadas en la configuración de PLU Inventory Counting y los parámetros recibidos. Esto permite obtener solo los LPs relevantes para el conteo.

3. **Recolecta de LPs y Jerarquía**: La API recolecta todos los LPs relacionados con las líneas filtradas y construye su jerarquía completa, incluyendo sus relaciones parent-child.

4. **Generación del JSON**: Se crea un objeto JSON que contiene la información completa del Warehouse Journal, los LPs y su jerarquía.

5. **Devolución del Resultado**: La API devuelve el JSON con el conteo físico de los LPs, incluyendo sus relaciones jerárquicas y los detalles de cada ítem.

### **7.4 Ventajas del Enfoque**

- **Trazabilidad Completa**: Registra todos los movimientos y relaciones de los LPs, garantizando una trazabilidad robusta.
- **Escalabilidad**: Permite manejar inventarios a gran escala con múltiples LPs jerárquicos.
- **Integración Sencilla**: Se puede integrar fácilmente con otros sistemas o procesos, tanto manuales como automáticos.

### **8. Resumen**

La gestión de License Plates (LPs) en Business Central mejora significativamente la eficiencia operativa de los almacenes al permitir la agrupación, división y manipulación de ítems bajo un identificador único. A través de la API `Get_WarehouseInvPhysicalCount_LP` y las operaciones sobre LPs como el split y el join, se garantiza una trazabilidad completa, flexibilidad en los movimientos y un control riguroso del inventario. Esto optimiza la gestión de grandes volúmenes de productos, asegurando la integridad y el control total del inventario en todo momento.

[[_TOSP_]]