### Documentación API: `GetAssignmentStatusForWarehousePick`

#### **Descripción general**
El método `GetAssignmentStatusForWarehousePick` se utiliza para obtener el estado de asignación de artículos en un proceso de **Warehouse Pick** (picking de almacén). Este método evalúa las líneas del picking para identificar cuántos artículos han sido asignados, cuántos aún faltan por asignar y si los artículos asignados cumplen con las cantidades requeridas por las líneas del pick. La respuesta se entrega en formato JSON, lo que permite una integración sencilla con otros sistemas.

#### **Estructura de la solicitud**
```json
{
  "ProcessMethod": "GetAssignmentStatusForWarehousePick",
  "Parameters": [
    {
      "WarehousePickNo": "WHSE PICK-03610"
    }
  ]
}
```

#### **Parámetros**
- **ProcessMethod**: El método a invocar, en este caso "GetAssignmentStatusForWarehousePick".
- **Parameters**: Un array que describe los parámetros necesarios para obtener el estado de asignación de artículos en el Warehouse Pick.
  - **WarehousePickNo**: El identificador único del Warehouse Pick que se está evaluando (por ejemplo, "WHSE PICK-03610").

#### **Flujo del proceso**
1. **Análisis de los parámetros**:
   - La API valida el `WarehousePickNo` proporcionado.
   
2. **Construcción de listas**:
   - El sistema construye una lista de artículos requeridos y una lista de artículos asignados para el Warehouse Pick especificado.
   
3. **Cálculo de cantidades**:
   - Para cada artículo requerido, el sistema evalúa cuántos han sido asignados y calcula las cantidades restantes.
   - Si todos los artículos requeridos están asignados correctamente, el artículo se marca como totalmente asignado.
   
4. **Generación de la respuesta**:
   - La API genera una respuesta en formato JSON con los detalles de los artículos requeridos, las cantidades asignadas y las cantidades que aún faltan por asignar.

#### **Ejemplo de solicitud**
```json
{
  "ProcessMethod": "GetAssignmentStatusForWarehousePick",
  "Parameters": [
    {
      "WarehousePickNo": "WHSE PICK-03610"
    }
  ]
}
```

#### **Ejemplo de respuesta**
```json
{
  "PickNo": "WHSE PICK-03610",
  "AssignmentStatus": [
    {
      "ItemNo": "ITEM123",
      "VariantCode": "VAR001",
      "QtyRequired": 5.0,
      "QtyAssigned": 5.0,
      "QtyRemaining": 0.0,
      "FullyAssigned": true
    },
    {
      "ItemNo": "ITEM456",
      "VariantCode": "VAR002",
      "QtyRequired": 10.0,
      "QtyAssigned": 7.0,
      "QtyRemaining": 3.0,
      "FullyAssigned": false
    }
  ]
}
```

#### **Campos de respuesta**
- **PickNo**: El número del Warehouse Pick evaluado (por ejemplo, `"WHSE PICK-03610"`).
- **AssignmentStatus**: Un array que contiene el estado de asignación de cada artículo en el Warehouse Pick:
  - **ItemNo**: El número del artículo (por ejemplo, `"ITEM123"`).
  - **VariantCode**: El código de variante del artículo, si aplica (por ejemplo, `"VAR001"`).
  - **QtyRequired**: La cantidad de artículos requerida en la línea del pick (por ejemplo, `5.0`).
  - **QtyAssigned**: La cantidad de artículos que ya han sido asignados (por ejemplo, `5.0`).
  - **QtyRemaining**: La cantidad de artículos que aún faltan por asignar (por ejemplo, `0.0` si ya está completamente asignado).
  - **FullyAssigned**: Un valor booleano que indica si la cantidad requerida ha sido completamente asignada (`true` si está totalmente asignado, `false` si no).

#### **Manejo de errores**
- Si el `WarehousePickNo` no es válido o no existe, la respuesta generará un error indicando que no se encontró el Warehouse Pick.
- Si ocurre un error inesperado durante el proceso de asignación, la API devolverá un mensaje de error detallado para su depuración.

#### **Consideraciones**
- **Validación de datos**: Es fundamental que el Warehouse Pick exista y que tenga líneas activas para poder realizar la asignación.
- **Eficiencia**: Este método está optimizado para manejar múltiples artículos y variantes de manera eficiente, calculando dinámicamente las cantidades asignadas y las pendientes.
  
#### **Resumen**
El método `GetAssignmentStatusForWarehousePick` permite obtener un estado detallado de las asignaciones en un Warehouse Pick en Business Central. Proporciona información clara sobre los artículos asignados y las cantidades restantes, permitiendo a los usuarios gestionar eficientemente los procesos de picking en el almacén y garantizando que las cantidades correctas sean asignadas a cada línea del pick.
