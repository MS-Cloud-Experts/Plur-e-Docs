# Documento del Proceso de Creación y Gestión de License Plates (LP)

## 1. Introducción

Este documento describe el enfoque para la creación y gestión de License Plates (LP) en Business Central. El objetivo es mejorar la automatización, la integridad de los datos y la eficiencia operativa en la gestión de inventarios dentro del almacén. Además, se detallan las operaciones sobre LPs, incluyendo split, join, movimientos entre bins, y otros procesos clave.

## 2. Principios Fundamentales y Estructura del Sistema

### 2.1 Un solo tipo de LP
Simplificación del sistema mediante un único tipo de LP capaz de contener ítems o relaciones con otros LPs.

### 2.2 Jerarquía Multinivel
Implementación de una jerarquía multinivel de LPs, permitiendo relaciones parent-child recursivas usando una tabla auxiliar de relaciones.

### 2.3 Eliminación del Tipo de Línea
Eliminación de la distinción entre líneas de ítems y líneas de LPs, utilizando una tabla de relaciones para manejar LPs hijos.

### 2.4 Uso de la Tabla LP Movements
Creación de una tabla auxiliar llamada LP Movements para rastrear todas las entradas y salidas de inventario relacionadas con un LP.

## 3. Estados de License Plates (LP)

1. **Pre-Labeled:** Estado inicial antes de la recepción. Un LP nuevo vacío que puede ser usado en cualquier proceso.
2. **Received:** Estado al crear el LP durante el registro del Warehouse Receipt.
3. **Labeled:** Estado durante el proceso de Put Away, generalmente en la zona de recepción.
4. **Stored:** Estado cuando el LP está en su ubicación de almacenamiento.
5. **Picked:** Estado cuando el LP ha sido seleccionado para envío.
6. **Packed:** Estado cuando el LP ha sido empaquetado para envío.
7. **Released:** Estado cuando el LP ha sido liberado para envío.
8. **Voided:** Estado cuando el LP ha sido anulado.
9. **Process:** Estado cuando el LP está en proceso de alguna operación.

## 4. Reglas de Integridad y Movimientos

1. **Integridad del Inventario:** Las cantidades totales en los LPs deben reflejar con exactitud las cantidades físicas.
2. **Restricciones de Capacidad:** Los LPs deben cumplir con las restricciones del bin en cuanto a capacidad y tipo de ítems.
3. **Movimientos de LPs:** Los movimientos se registran en la tabla "PLU LP Movements" para mantener la trazabilidad.
4. **Compatibilidad de Estados:** Solo se pueden unir LPs que estén en estados que permitan la consolidación, como "Stored" o "Received". Los LPs en estados "Blocked" o "Reserved" deben ser excluidos del proceso.

## 5. Procesos de Entrada y Salida

### 5.1 Procesos de Entrada

#### **Warehouse Receipt**
- **Recepción de Mercancías:** Los LPs se crean con el estado "Received" al registrar un Warehouse Receipt.
- **Posteo del Warehouse Receipt:** Se genera una entrada en la tabla de LP Movements y el estado del LP cambia a "Labeled".

### 5.2 Procesos de Salida

#### **Warehouse Shipments**
- **Por Definir:** Aquí se detallarán los procesos de salida relacionados con los envíos.

### 5.3 Procesos de Ambas (Entrada y Salida)

#### **Warehouse Item Journal**
- **Creación de LPs:** Los LPs se crean al registrar líneas en el Warehouse Item Journal.
- **Posteo del Warehouse Item Journal:** Se registran los movimientos asociados al LP.

#### **Warehouse Physical Inventory Journal**
- **Inventario Físico:** Se crean LPs para los productos encontrados durante el inventario físico.
- **Posteo del Warehouse Physical Inventory Journal:** Se actualizan las cantidades de los LPs y se registran en la tabla de LP Movements.

## 6. Operaciones sobre License Plates (LP)

### 6.1 Proceso de Split de LPs

- **Descripción:** División de un LP en varios nuevos LPs.
- **Reglas y Ejemplos:** Descripción de escenarios como el split de un LP con una o múltiples líneas de ítems, y el manejo de LPs hijos durante el split.

### 6.2 Proceso de Join (Unión) de LPs

- **Descripción:** Unión de varios LPs en uno solo para consolidar inventarios.
- **Flujo del Proceso:** Selección de LPs, definición del LP destino, transferencia de cantidades, registro de movimientos, y actualización de estados.

### 6.3 Proceso Bin to Bin (Movimientos entre Bins) de License Plates

- **Descripción:** Transferencia de LPs de un bin a otro dentro del almacén.
- **Flujo del Proceso:** Selección de LPs, validación de bins, ejecución del movimiento, posteo, y actualización de registros.

### 6.4 Proceso Get Bin Content (Obtener Contenido del Bin)

- **Objetivo:** Consultar el contenido de un bin específico, incluyendo los LPs y las cantidades asociadas.
- **Flujo del Proceso:** Selección del bin, consulta de la tabla PLU LP Movements, presentación de datos.

## 7. Consideraciones Adicionales

### 7.1 Auditoría y Trazabilidad

El proceso de unión debe ser completamente trazable, con registros detallados de los movimientos y cambios de estado en el inventario.

### 7.2 Compatibilidad de Estados

Solo se pueden unir LPs que estén en estados que permitan la consolidación, como "Stored" o "Received". Los LPs en estados "Blocked" o "Reserved" deben ser excluidos del proceso.

### 7.3 Ventas

Para los procesos de ventas, se requiere un proceso de **Assemblies** para construir **Kits** que automáticamente busquen sustitutos si al momento de vender no hay disponibilidad de uno de sus productos.

### Indice


[[_TOSP_]]
