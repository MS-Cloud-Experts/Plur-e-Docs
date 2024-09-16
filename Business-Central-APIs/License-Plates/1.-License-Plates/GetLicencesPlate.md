### API Documentation: GetLicencesPlate

#### **Overview**
El método `GetLicencesPlate` permite obtener los detalles de los License Plates (LPs) dentro de un sistema de gestión de almacenes en Business Central. Esta API procesa los parámetros de entrada en formato JSON y devuelve una estructura detallada de los LPs que coinciden con el filtro. La respuesta incluye información clave como el estado del LP, ubicación, cantidades, y la jerarquía de LPs relacionados.

#### **Request Structure**
```json
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP-00097"
    }
  ]
}
```

#### **Parameters**
- **ProcessMethod**: El nombre del método a invocar, en este caso `"GetLicencesPlate"`.
- **Parameters**: Un array de objetos que contiene los filtros para la búsqueda de License Plates.
  - **No**: El número de documento del License Plate que se desea consultar (e.g., `"LP-00097"`).

#### **Example Request**
```json
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP-00097"
    }
  ]
}
```

#### **Example Response**
```json
{
  "LicensePlates": [
    {
      "LPDocumentNo": "LP-00097",
      "LicensePlateStatus": "Stored",
      "ParentLPNo": "",
      "ZoneCode": "STO",
      "LocationCode": "NEWWMS",
      "BinCode": "STO-3",
      "WhseDocumentNo": "WHSE REC-00093",
      "SystemCreatedAt": "2024-09-03T20:53:31.7670000Z",
      "SystemCreatedBy": "{2BEFFABC-4F0A-40E0-8454-4F8B442532AF}",
      "LPTotalQuantities": 5.0,
      "LPLines": [
        {
          "LineNo": 10000,
          "ItemNo": "1010",
          "VariantCode": "",
          "SerialNo": "",
          "LotNo": "",
          "Description": "",
          "Quantity": 3.0,
          "UnitofMeasure": "PCS",
          "SourceWhseLineNo": 10000
        },
        {
          "LineNo": 20000,
          "ItemNo": "1010",
          "VariantCode": "",
          "SerialNo": "",
          "LotNo": "",
          "Description": "",
          "Quantity": 2.0,
          "UnitofMeasure": "PCS",
          "SourceWhseLineNo": 10000
        }
      ],
      "ChildLPs": [
        {
          "ChildLPDocumentNo": "LP-00116",
          "ChildLPStatus": "Stored",
          "ZoneCode": "STO",
          "LocationCode": "NEWWMS",
          "BinCode": "STO-3",
          "WhseDocumentNo": "WHSE REC-00096",
          "SystemCreatedAt": "2024-09-09T12:27:58.2830000Z",
          "SystemCreatedBy": "{2BEFFABC-4F0A-40E0-8454-4F8B442532AF}",
          "ChildLPTotalQuantities": 2.0,
          "LPLines": [
            {
              "LineNo": 10000,
              "ItemNo": "1010",
              "VariantCode": "",
              "SerialNo": "",
              "LotNo": "",
              "Description": "",
              "Quantity": 2.0,
              "UnitofMeasure": "PCS",
              "SourceWhseLineNo": 10000
            }
          ],
          "ChildLPs": []
        }
      ]
    }
  ],
  "Duration": "101 milliseconds"
}
```

#### **Explanation**
- **LicensePlates**: Un array que contiene los detalles de los License Plates encontrados.
  - **LPDocumentNo**: El número del documento del License Plate (e.g., `"LP-00097"`).
  - **LicensePlateStatus**: El estado actual del LP (e.g., `"Stored"`).
  - **ParentLPNo**: El número del License Plate padre, si existe (e.g., `""`).
  - **ZoneCode**: El código de la zona donde se encuentra el LP (e.g., `"STO"`).
  - **LocationCode**: El código de la ubicación del almacén (e.g., `"NEWWMS"`).
  - **BinCode**: El código del bin donde está almacenado el LP (e.g., `"STO-3"`).
  - **WhseDocumentNo**: El número del documento del almacén relacionado (e.g., `"WHSE REC-00093"`).
  - **SystemCreatedAt**: La fecha y hora de creación del LP (e.g., `"2024-09-03T20:53:31.7670000Z"`).
  - **SystemCreatedBy**: El usuario o sistema que creó el LP (e.g., `"{2BEFFABC-4F0A-40E0-8454-4F8B442532AF}"`).
  - **LPTotalQuantities**: La cantidad total asociada al License Plate (e.g., `5.0`).
  - **LPLines**: Un array con las líneas del LP, que detalla los ítems asociados al LP.
    - **LineNo**: El número de la línea en el documento del LP (e.g., `10000`).
    - **ItemNo**: El número de ítem (e.g., `"1010"`).
    - **Quantity**: La cantidad del ítem en esta línea (e.g., `3.0`).
  - **ChildLPs**: Un array que contiene los LPs hijos relacionados con el LP principal, incluyendo sus detalles.

#### **Summary**
El método `GetLicencesPlate` devuelve la estructura jerárquica de License Plates en un almacén de Business Central, proporcionando detalles como el estado, cantidades y ubicación de los LPs, así como sus relaciones con LPs hijos. Este método asegura la trazabilidad completa de los License Plates y es útil para auditorías y reconciliaciones de inventario.

### Lógica de Implementación
1. **Validación de Parámetros**: 
   - La API valida los parámetros de entrada para asegurarse de que el número de documento del LP es correcto.
   
2. **Consulta de License Plates**:
   - El sistema consulta las tablas de LP utilizando el número de documento proporcionado en los parámetros.
   
3. **Formateo de Respuesta en JSON**:
   - Si se encuentran LPs, la respuesta incluye el detalle de los LPs y su jerarquía.
   - Si no se encuentran registros, se lanza un error.

4. **Devolución del JSON**: 
   - La API genera la estructura JSON con la información solicitada y la devuelve al solicitante.