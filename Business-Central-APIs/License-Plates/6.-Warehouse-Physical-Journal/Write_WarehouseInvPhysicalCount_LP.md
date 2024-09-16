### API Documentation: Write_WarehouseInvPhysicalCount_LP

#### **Overview**
El método `Write_WarehouseInvPhysicalCount_LP` permite escribir datos relacionados con el conteo físico de inventario de License Plates (LPs) en un Warehouse Journal en Business Central. La API procesa los parámetros de entrada en formato JSON, inserta y valida las líneas en el Warehouse Journal, y actualiza el inventario de acuerdo con los datos proporcionados.

#### **Request Structure**
```json
{
  "ProcessMethod": "Write_WarehouseInvPhysicalCount_LP",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DEFAULT",
      "LineNo": 10000,
      "RegisteringDate": "2024-09-12",
      "LocationCode": "MAIN",
      "ItemNo": "D0AVESVTBLU00S",
      "QtyPhysInventory": 2.0,
      "ZoneCode": "STORAGE",
      "BinCode": "1001",
      "UserID": "IVAN.LABRADOR",
      "VariantCode": "",
      "SerialNo": "",
      "LotNo": "",
      "LPDocumentNo": "LP-00033",
      "LPLine": "10000",
    },
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DEFAULT",
      "LineNo": 20000,
      "RegisteringDate": "2024-09-12",
      "LocationCode": "MAIN",
      "ItemNo": "D0BDBD",
      "QtyPhysInventory": 2.0,
      "ZoneCode": "STORAGE",
      "BinCode": "1001",
      "UserID": "IVAN.LABRADOR",
      "VariantCode": "B60W225",
      "SerialNo": "",
      "LotNo": "",
      "IsInitial": false,
      "LPDocumentNo": "LP-00034",
      "LPLine": "10000",
    }
    // ... more lines ...
  ]
}
```

#### **Parameters**
- **ProcessMethod**: El método a invocar, en este caso `"Write_WarehouseInvPhysicalCount_LP"`.
- **Parameters**: Un array de objetos que contiene la información de las líneas del Warehouse Journal para ser escritas o actualizadas.
  - **JournalTemplateName**: El nombre de la plantilla del Warehouse Journal (e.g., `"PHYSICAL I"`).
  - **JournalBatchName**: El nombre del batch del Warehouse Journal (e.g., `"DEFAULT"`).
  - **LineNo**: El número de línea dentro del Warehouse Journal (e.g., `10000`).
  - **RegisteringDate**: La fecha en que se está registrando el conteo físico (e.g., `"2024-09-12"`).
  - **LocationCode**: El código de la ubicación del almacén donde se realiza el conteo (e.g., `"MAIN"`).
  - **ItemNo**: El número de ítem para el cual se está haciendo el conteo (e.g., `"D0AVESVTBLU00S"`).
  - **QtyPhysInventory**: La cantidad física del inventario contada (e.g., `2.0`).
  - **ZoneCode**: El código de la zona donde se encuentra el ítem (e.g., `"STORAGE"`).
  - **BinCode**: El código del bin donde está almacenado el ítem (e.g., `"1001"`).
  - **UserID**: El ID del usuario que está realizando la operación (e.g., `"IVAN.LABRADOR"`).
  - **VariantCode**: El código de variante del ítem, si aplica (e.g., `""`).
  - **SerialNo**: El número de serie del ítem, si aplica (e.g., `""`).
  - **LotNo**: El número de lote del ítem, si aplica (e.g., `""`).
  - **IsInitial**: Booleano que indica si este es el conteo inicial (e.g., `false`).
  - **LPDocumentNo**: El número de documento del License Plate asociado (e.g., `"LP-00033"`).

#### **Example Request**
```json
{
  "ProcessMethod": "Write_WarehouseInvPhysicalCount_LP",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DEFAULT",
      "LineNo": 10000,
      "RegisteringDate": "2024-09-12",
      "LocationCode": "MAIN",
      "ItemNo": "D0AVESVTBLU00S",
      "QtyPhysInventory": 2.0,
      "ZoneCode": "STORAGE",
      "BinCode": "1001",
      "UserID": "IVAN.LABRADOR",
      "VariantCode": "",
      "SerialNo": "",
      "LotNo": "",
      "IsInitial": false,
      "LPDocumentNo": "LP-00033"
    }
  ]
}
```

#### **Example Response**
```json
{
  "WarehouseInvPhysicalCount_LP": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DEFAULT",
      "BinCode": "1001",
      "LineNo": 10000,
      "RegisteringDate": "2024-09-12",
      "LocationCode": "MAIN",
      "ItemNo": "D0AVESVTBLU00S",
      "UnitofMeasureCode": "EA",
      "QtyPhysInventory": 2.0,
      "QtyCalculatedBase": 2.0,
      "UserID": "IVAN.LABRADOR",
      "VariantCode": "",
      "SerialNo": "",
      "LotNo": "",
      "ZoneCode": "STORAGE",
      "ExpirationDate": "0001-01-01",
      "LPDocumentNo": "LP-00033",
      "SuperParentLP": "LP-00033",
      "LPHierarchy": {
        "LPDocumentNo": "LP-00033",
        "LicensePlateStatus": "Stored",
        "ParentLPNo": "",
        "ZoneCode": "STORAGE",
        "LocationCode": "MAIN",
        "BinCode": "1001",
        "WhseDocumentNo": "WHSE REC-00211",
        "SystemCreatedAt": "2024-09-10T13:39:43.0900000Z",
        "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
        "LPTotalQuantities": 2.0,
        "LPLines": [
          {
            "LineNo": 10000,
            "ItemNo": "D0AVESVTBLU00S",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "",
            "Quantity": 2.0,
            "UnitofMeasure": "EA",
            "SourceWhseLineNo": 10000
          }
        ],
        "ChildLPs": []
      }
    }
  ],
  "Duration": "163 milliseconds"
}
```

#### **Explanation**
- **WarehouseInvPhysicalCount_LP**: Un array que contiene las líneas actualizadas del Warehouse Journal y los detalles de los License Plates asociados.
  - **JournalTemplateName**: El nombre de la plantilla del Warehouse Journal (e.g., `"PHYSICAL I"`).
  - **JournalBatchName**: El nombre del batch del Warehouse Journal (e.g., `"DEFAULT"`).
  - **BinCode**: El código del bin donde está almacenado el ítem (e.g., `"1001"`).
  - **LineNo**: El número de línea dentro del Warehouse Journal (e.g., `10000`).
  - **RegisteringDate**: La fecha de registro (e.g., `"2024-09-12"`).
  - **LocationCode**: El código de la ubicación del almacén (e.g., `"MAIN"`).
  - **ItemNo**: El número del ítem (e.g., `"D0AVESVTBLU00S"`).
  - **UnitofMeasureCode**: El código de la unidad de medida (e.g., `"EA"`).
  - **QtyPhysInventory**: La cantidad física registrada en el inventario (e.g., `2.0`).
  - **QtyCalculatedBase**: La cantidad calculada en la unidad base (e.g., `2.0`).
  - **UserID**: El usuario que realizó la operación (e.g., `"IVAN.LABRADOR"`).
  - **LPHierarchy**: La jerarquía del License Plate relacionado, incluyendo ítems y LPs hijos.

#### **Summary**
El método `Write_WarehouseInvPhysicalCount_LP` permite escribir datos relacionados con el conteo físico de License Plates (LPs) en el Warehouse Journal, insertando o actualizando líneas según los parámetros proporcionados. La API asegura la correcta inserción de los datos y genera una respuesta detallada que incluye los License Plates y su jerarquía relacionada.

### Lógica de Implementación
1. **Validación de Parámetros**: 
   - Se verifica que todos los campos requeridos, como el número de ítem y cantidad física, estén presentes y correctamente formateados.

2. **Inserción/Actualización de Líneas**:
   - Si se proporcionan líneas nuevas, se insertan en el Warehouse Journal.
   - Si las líneas ya existen, se actualizan

 con las nuevas cantidades físicas.

3. **Generación del JSON de Respuesta**:
   - La API genera un objeto JSON con la información actualizada del Warehouse Journal y los License Plates asociados.

4. **Retorno de Respuesta**:
   - El JSON final es devuelto al cliente, incluyendo la jerarquía completa de los License Plates, permitiendo una trazabilidad total.