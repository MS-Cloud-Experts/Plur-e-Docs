### API Documentation: CreateEmptyLPFromWarehousePick

#### Overview
El método `CreateEmptyLPFromWarehousePick` permite la creación de un License Plate (LP) vacío vinculado a un Warehouse Pick específico. Este proceso es especialmente útil para prepararse para futuras funcionalidades, como la integración con plataformas de envío (por ejemplo, Starship o ShipStation), y permite una mayor flexibilidad en la gestión de inventario durante las operaciones de picking en el almacén.

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
