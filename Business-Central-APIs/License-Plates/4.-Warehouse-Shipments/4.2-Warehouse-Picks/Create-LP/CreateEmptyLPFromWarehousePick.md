### API Documentation: CreateEmptyLPFromWarehousePick

#### Overview
El método AssignItemToLPFromWarehousePick asigna un artículo a un License Plate (LP) desde una línea específica de Warehouse Pick. Este proceso es aplicable solo para artículos o variantes que no dispongan de LPs existentes en estado Storage, lo cual asegura que se creen LPs únicamente para items sin asignación previa en almacenamiento. Para utilizar este método, es necesario que el LP header haya sido creado previamente; para más información, consulte la documentación de CreateEmptyLPFromWarehousePick.

Esta funcionalidad permite una gestión de inventario precisa y está diseñada para soportar futuras funciones, como la integración con plataformas de envío (e.g., Starship, ShipStation).

#### Request Structure
```json
{
  "ProcessMethod": "CreateEmptyLPFromWarehousePick",
  "Parameters": [
    {
      "PickNo": "PK-001"
    }
  ]
}
```

#### Parameters
- **PickNo**: El número del Warehouse Pick al que se vinculará el LP vacío (e.g., `"PK-001"`).

#### Example Request
```json
{
  "ProcessMethod": "CreateEmptyLPFromWarehousePick",
  "Parameters": [
    {
      "PickNo": "PK-002"
    }
  ]
}
```

#### Example Response
```json
{
  "LPDocumentNo": "LP-EMPTY-002",
  "Message": "An empty LP was created and linked to Warehouse Pick PK-002 successfully.",
  "Duration": "2 seconds 564 milliseconds"
}
```

#### Explanation
- **LPDocumentNo**: El número de documento del License Plate vacío creado.
- **Message**: Mensaje de confirmación indicando que el LP vacío se creó y vinculó con éxito al Warehouse Pick especificado.

#### Additional Information
Para insertar items en el License Plate (LP) creado, refiérase a la documentación de `AssignItemToLPFromWarehousePick`, disponible en [este enlace](https://dev.azure.com/MSCloudExperts/Plur-e/_wiki/wikis/Plur-e.wiki/649/AssignItemToLPFromWarehousePick).

#### Summary
El método `CreateEmptyLPFromWarehousePick` es fundamental para generar LPs vacíos asociados a un Warehouse Pick, una funcionalidad diseñada para soportar futuras integraciones con sistemas de envío. Este proceso permite un flujo más flexible en la operación del almacén, brindando capacidad para gestionar picking y envíos en un ciclo optimizado de inventario.

