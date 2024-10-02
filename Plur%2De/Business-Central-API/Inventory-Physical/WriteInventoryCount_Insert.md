### Documentación de la API: WriteInventoryCount_Insert

#### **Descripción General**
El método `WriteInventoryCount_Insert` permite insertar entradas de conteo físico de inventario en el diario de artículos. Procesa múltiples líneas del diario de artículos, incluyendo números de serie si aplican, y registra estos conteos en el diario de inventario físico. Además, asegura que se refleje cualquier discrepancia entre el conteo físico y las cantidades calculadas por el sistema, actualizando correctamente el inventario en Business Central.

Este metodo se utiliza cuando no existen lineas en el Batch y cada vez que se ejecute borra las lineas y las vuelve a crear.

#### **Estructura de la Solicitud**
```json
{
  "ProcessMethod": "WriteInventoryCount_Insert",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-13",
      "DocumentNo": "SSDS",
      "ItemNo": "70001",
      "VariantCode": "",
      "Description": "",
      "LocationCode": "ASIA TEMP",
      "SalespersPurchCode": "",
      "QtyPhysInventory": 2,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "SerialJA": [
        {
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "ELLOTE",
          "SerialNo": "X14q",
          "ExpirationDate" : "2024-10-01"
        },
        {
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "ELLOTE",
          "SerialNo": "X15q",
          "ExpirationDate" : "2024-10-01"
        }
      ]
    },
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-13",
      "DocumentNo": "SSDS",
      "ItemNo": "70001",
      "VariantCode": "",
      "Description": "",
      "LocationCode": "ASIA TEMP",
      "SalespersPurchCode": "",
      "QtyPhysInventory": 2,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "SerialJA": [
        {
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "ELLOTE",
          "SerialNo": "X14",
          "ExpirationDate" : "2024-10-01"
        },
        {
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "ELLOTE",
          "SerialNo": "X15",
          "ExpirationDate" : "2024-10-01"
        }
      ]
    }
  ]
}
```

#### **Parámetros**
- **ProcessMethod**: Indica el método a invocar, en este caso `"WriteInventoryCount_Insert"`.
- **Parameters**: Un array de objetos que describen las líneas del diario de inventario.
  - **JournalTemplateName**: El nombre de la plantilla de diario utilizada (e.g., `"PHYS. INV."`).
  - **JournalBatchName**: El nombre del lote de diario (e.g., `"DEFAULT"`).
  - **PostingDate**: La fecha de registro de la entrada en el diario (e.g., `"2024-06-13"`).
  - **DocumentNo**: El número de documento para esta entrada (e.g., `"SSDS"`).
  - **ItemNo**: El número de artículo que se está procesando (e.g., `"SERIAL2"`).
  - **VariantCode**: El código de variante del artículo, si aplica (e.g., `"T0MLXXX"`).
  - **Description**: Una descripción del artículo.
  - **LocationCode**: El código de la ubicación donde está almacenado el artículo (e.g., `"ASIA TEMP"`).
  - **SalespersPurchCode**: El código del vendedor o comprador, si aplica.
  - **QtyPhysInventory**: La cantidad física de inventario contada (e.g., `1322`).
  - **UserID**: El ID del usuario que procesó esta entrada.
  - **TimeStampMovil**: Un timestamp para el procesamiento móvil (e.g., `"2024-06-13T00:00:00"`).
  - **SerialJA**: Un array de números de serie si el artículo tiene seguimiento por número de serie.

#### **Consideraciones Importantes**
1. **La variante del `SerialJA` debe coincidir con la variante del artículo**:
   - Para evitar errores o la creación incorrecta de la línea del diario, el código de variante especificado en cada número de serie dentro del array `SerialJA` **debe coincidir** con el código de variante del artículo en la línea principal. Si la variante del número de serie no coincide con la variante del artículo, el sistema puede generar un error o crear la línea incorrectamente.
   
   Por ejemplo:
   ```json
   {
     "ItemNo": "SERIAL2",
     "VariantCode": "T0MLXXX",
     "SerialJA": [
       {
         "LineNo": 10000,
         "VariantCode": "T0MLXXX",  // Debe coincidir con la línea principal
         "SerialNo": "X14q"
       }
     ]
   }
   ```

2. **La cantidad de `QtyPhysInventory` debe coincidir con la cantidad de elementos en el array `SerialJA`**:
   - Si el artículo tiene números de serie, el valor de `QtyPhysInventory` debe ser igual al número total de elementos en el array `SerialJA`. Si no coinciden, se generará una inconsistencia entre la cantidad física y el número de series asociadas al artículo.
   
   Por ejemplo, si `QtyPhysInventory` es 2, debe haber exactamente 2 elementos en `SerialJA`:
   ```json
   "QtyPhysInventory": 2,
   "SerialJA": [
     {
       "SerialNo": "X14q"
     },
     {
       "SerialNo": "X15q"
     }
   ]
   ```

#### **Ejemplo de Respuesta**
```json
{
  "WriteInventoryCount_Insert": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "DEFAULT",
      "PostingDate": "2024-06-13",
      "EntryType": "Positive Adjmt.",
      "DocumentNo": "SSDS",
      "ItemNo": "SERIAL2",
      "VariantCode": "",
      "Description": "C.O.S OVERDRIVE TRIMLITE",
      "LocationCode": "ASIA",
      "SalespersPurchCode": "",
      "QtyCalculated": 0.0,
      "QtyPhysInventory": 2.0,
      "Quantity": 2.0,
      "UserID": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
      "LineNo": 10000,
      "BinCode": "",
      "UnitofMeasureCode": "EA",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "UncountedSerialsJA": [],
      "CountedSerialsJA": [
        {
          "SerialNo": "X141"
        },
        {
          "SerialNo": "X151"
        }
      ]
    }
  ],
  "Duration": "46 seconds 535 milliseconds"
}
```

#### **Explicación**
- **WriteInventoryCount_Insert**: Una lista de líneas del diario de artículos que han sido procesadas.
  - **JournalTemplateName**: El nombre de la plantilla de diario utilizada.
  - **JournalBatchName**: El nombre del lote de diario.
  - **PostingDate**: La fecha de registro de la entrada en el diario.
  - **EntryType**: El tipo de entrada, como "Positive Adjmt." (Ajuste Positivo).
  - **DocumentNo**: El número de documento para la entrada en el diario.
  - **ItemNo**: El número de artículo para la entrada.
  - **VariantCode**: El código de variante del artículo, si aplica.
  - **Description**: La descripción del artículo.
  - **LocationCode**: El código de la ubicación donde está almacenado el artículo.
  - **QtyCalculated**: La cantidad calculada por el sistema.
  - **QtyPhysInventory**: La cantidad física de inventario que fue contada.
  - **Quantity**: La cantidad final del artículo en el diario.
  - **UserID**: El ID del usuario que procesó la entrada.
  - **LineNo**: El número de línea de la entrada en el diario.
  -