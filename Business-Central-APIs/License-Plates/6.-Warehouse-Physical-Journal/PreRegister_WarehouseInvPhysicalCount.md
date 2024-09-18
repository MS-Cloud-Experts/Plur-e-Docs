### Documentación de API: `PreRegister_WarehouseInvPhysicalCount`

#### **Visión General**
El método `PreRegister_WarehouseInvPhysicalCount` procesa las líneas del diario de inventario físico de un almacén, identificando y gestionando aquellas líneas que fueron sobrecontadas o subcontadas. Este método gestiona las placas de licencia (License Plates, LPs) y sus líneas relacionadas (padre-hijo), transfiriendo la información a un nuevo lote de diario para revisión, garantizando la integridad del inventario durante el proceso de conteo.

#### **Estructura de la Solicitud**
```json
{
  "ProcessMethod": "PreRegister_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DEFAULT",
      "LocationCode": "MAIN",
      "WsheJournalBatchDobleCheckName": "IVAN-RVIEW"
    }
  ]
}
```

#### **Parámetros**
- **ProcessMethod**: El método a invocar, en este caso `"PreRegister_WarehouseInvPhysicalCount"`.
- **Parameters**: Un array de objetos que contiene los siguientes filtros:
  - **JournalTemplateName**: Nombre de la plantilla del diario de inventario (e.g., `"PHYSICAL I"`).
  - **JournalBatchName**: Nombre del lote del diario de inventario (e.g., `"IVAN"`).
  - **LocationCode**: Código de la ubicación del almacén (e.g., `"NEWWMS"`).
  - **WsheJournalBatchDobleCheckName**: Nombre del nuevo lote para la revisión de líneas (e.g., `"IVAN-REVIEW"`).

#### **Ejemplo de Solicitud**
```json
{
  "ProcessMethod": "PreRegister_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DEFAULT",
      "LocationCode": "MAIN",
      "WsheJournalBatchDobleCheckName": "IVAN-RVIEW"
    }
  ]
}
```

#### **Ejemplo de Respuesta**
```json
{
  "Warehouse_Physical_Inventory_Counted": {
    "WarehouseInvPhysicalCount_LP": [
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 40000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00020",
        "LPLineNo": 30000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 50000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00022",
        "LPLineNo": 30000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 60000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 5.0,
        "QtyCalculatedBase": 5.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00023",
        "LPLineNo": 60000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 70000,
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
        "LPDocumentNo": "LP-00028",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 80000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 7.0,
        "QtyCalculatedBase": 7.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00028",
        "LPLineNo": 40000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 90000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 12.0,
        "QtyCalculatedBase": 12.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00029",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 100000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00042",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 110000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "1",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00023",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 120000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "1A1A1A77711A57",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00041",
        "LPLineNo": 30000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 130000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "1A1A1A777Q11A57",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00041",
        "LPLineNo": 40000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 140000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "2",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00023",
        "LPLineNo": 20000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 150000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "4",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00023",
        "LPLineNo": 40000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 160000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "5",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00023",
        "LPLineNo": 50000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 170000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "A1A10",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 100000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 180000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "A1A5",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 50000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 190000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "A1A6",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 60000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 200000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "A1A7",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 70000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 210000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "A1A8",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 80000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 220000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "A1A9",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 90000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 230000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "AAA",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00028",
        "LPLineNo": 20000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 240000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "BBB",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00028",
        "LPLineNo": 30000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 250000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "QWEWQEWEQ1",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00020",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 260000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "QWEWQEWEQ2",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00020",
        "LPLineNo": 20000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 270000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "NMEDXXX",
        "SerialNo": "AAA1A111A1",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00043",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00043"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 280000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "ITEM SERIAL TEST",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "NMEDXXX",
        "SerialNo": "NMEDXXX",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00030",
        "LPLineNo": 110000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 290000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "K4WBCODEX",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "411XXX",
        "SerialNo": "1SNA001XX",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00041",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00042"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "DEFAULT",
        "BinCode": "BACK",
        "LineNo": 300000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "K4WBCODEX",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "411XXX",
        "SerialNo": "1SNA002XX",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00041",
        "LPLineNo": 20000,
        "SuperParentLP": "LP-00042"
      }
    ],
    "LPArray": [
      {
        "SuperParentLP": "LP-00042",
        "LPHierarchy": {
          "LPDocumentNo": "LP-00042",
          "LicensePlateStatus": "Stored",
          "ParentLPNo": "",
          "ZoneCode": "STORAGE",
          "LocationCode": "MAIN",
          "BinCode": "BACK",
          "WhseDocumentNo": "WHSE REC-00210",
          "SystemCreatedAt": "2024-09-11T16:04:55.8400000Z",
          "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
          "LPTotalQuantities": 1.0,
          "LPLines": [
            {
              "LineNo": 10000,
              "ItemNo": "D0AVESVTBLU00S",
              "VariantCode": "",
              "SerialNo": "",
              "LotNo": "",
              "Description": "",
              "Quantity": 1.0,
              "UnitofMeasure": "EA",
              "SourceWhseLineNo": 0
            }
          ],
          "ChildLPs": [
            {
              "ChildLPDocumentNo": "LP-00020",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "BACK",
              "WhseDocumentNo": "",
              "SystemCreatedAt": "2024-09-06T21:14:00.7270000Z",
              "SystemCreatedBy": "{12EDC3D8-902A-49B3-A686-704C1269CA0C}",
              "ChildLPTotalQuantities": 3.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "QWEWQEWEQ1",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "QWEWQEWEQ2",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "D0AVESVTBLU00S",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            },
            {
              "ChildLPDocumentNo": "LP-00022",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "BACK",
              "WhseDocumentNo": "",
              "SystemCreatedAt": "2024-09-09T16:01:16.3900000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 1.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "B",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "D0AVESVTBLU00S",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            },
            {
              "ChildLPDocumentNo": "LP-00023",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "BACK",
              "WhseDocumentNo": "",
              "SystemCreatedAt": "2024-09-09T16:45:54.9830000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 13.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "1",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "2",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "3",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 40000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "4",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 50000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "5",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 60000,
                  "ItemNo": "D0AVESVTBLU00S",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 5.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 70000,
                  "ItemNo": "D0AVESVTBLU00S",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 2.0,
                  "UnitofMeasure": "",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 80000,
                  "ItemNo": "DK22W32RTS",
                  "VariantCode": "10",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 90000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "NMEDXXX",
                  "SerialNo": "1010101",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            },
            {
              "ChildLPDocumentNo": "LP-00028",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "BACK",
              "WhseDocumentNo": "",
              "SystemCreatedAt": "2024-09-09T21:20:15.9700000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 11.0,
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
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "AAA",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "BBB",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 40000,
                  "ItemNo": "D0AVESVTBLU00S",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 7.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            },
            {
              "ChildLPDocumentNo": "LP-00029",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "BACK",
              "WhseDocumentNo": "",
              "SystemCreatedAt": "2024-09-09T22:24:39.6200000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 12.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "D0AVESVTBLU00S",
                  "VariantCode": "",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 12.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "AAA11",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "T0MLXXX",
                  "SerialNo": "1321321231A",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 40000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "IVANSERIAL",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            },
            {
              "ChildLPDocumentNo": "LP-00030",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "BACK",
              "WhseDocumentNo": "",
              "SystemCreatedAt": "2024-09-09T22:53:18.7770000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 7.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A1",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A2",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A3",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 40000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A4",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 0.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 50000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A5",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 60000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A6",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 70000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A7",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 80000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A8",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 90000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A9",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 100000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "A1A10",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 110000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "NMEDXXX",
                  "SerialNo": "NMEDXXX",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            },
            {
              "ChildLPDocumentNo": "LP-00041",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "",
              "WhseDocumentNo": "WHSE REC-00210",
              "SystemCreatedAt": "2024-09-11T16:04:50.1530000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 4.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "K4WBCODEX",
                  "VariantCode": "411XXX",
                  "SerialNo": "1SNA001XX",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 20000
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "K4WBCODEX",
                  "VariantCode": "411XXX",
                  "SerialNo": "1SNA002XX",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 20000
                },
                {
                  "LineNo": 30000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "1A1A1A77711A57",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                },
                {
                  "LineNo": 40000,
                  "ItemNo": "ITEM SERIAL TEST",
                  "VariantCode": "",
                  "SerialNo": "1A1A1A777Q11A57",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            }
          ]
        }
      },
      {
        "SuperParentLP": "LP-00043",
        "LPHierarchy": {
          "LPDocumentNo": "LP-00043",
          "LicensePlateStatus": "Stored",
          "ParentLPNo": "",
          "ZoneCode": "STORAGE",
          "LocationCode": "MAIN",
          "BinCode": "BACK",
          "WhseDocumentNo": "",
          "SystemCreatedAt": "2024-09-17T21:02:51.3430000Z",
          "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
          "LPTotalQuantities": 1.0,
          "LPLines": [
            {
              "LineNo": 10000,
              "ItemNo": "ITEM SERIAL TEST",
              "VariantCode": "NMEDXXX",
              "SerialNo": "AAA1A111A1",
              "LotNo": "",
              "Description": "",
              "Quantity": 1.0,
              "UnitofMeasure": "EA",
              "SourceWhseLineNo": 0
            }
          ],
          "ChildLPs": []
        }
      }
    ]
  },
  "Warehouse_Physical_Inventory_NoCounted": {
    "WarehouseInvPhysicalCount_LP": [
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "IVAN-RVIEW",
        "BinCode": "1001",
        "LineNo": 10000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0AVESVTBLU00S",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 2.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00033",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00033"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "IVAN-RVIEW",
        "BinCode": "1001",
        "LineNo": 20000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0BDBD",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 2.0,
        "QtyCalculatedBase": 2.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "B60W225",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00034",
        "LPLineNo": 10000,
        "SuperParentLP": "LP-00033"
      },
      {
        "JournalTemplateName": "PHYSICAL I",
        "JournalBatchName": "IVAN-RVIEW",
        "BinCode": "1001",
        "LineNo": 30000,
        "RegisteringDate": "2024-09-12",
        "LocationCode": "MAIN",
        "ItemNo": "D0BDBD",
        "UnitofMeasureCode": "EA",
        "QtyPhysInventory": 1.0,
        "QtyCalculatedBase": 1.0,
        "UserID": "IVAN.LABRADOR",
        "VariantCode": "B60W225",
        "SerialNo": "",
        "LotNo": "",
        "ZoneCode": "STORAGE",
        "ExpirationDate": "0001-01-01",
        "LPDocumentNo": "LP-00034",
        "LPLineNo": 20000,
        "SuperParentLP": "LP-00033"
      }
    ],
    "LPArray": [
      {
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
          "ChildLPs": [
            {
              "ChildLPDocumentNo": "LP-00034",
              "ChildLPStatus": "Stored",
              "ZoneCode": "STORAGE",
              "LocationCode": "MAIN",
              "BinCode": "",
              "WhseDocumentNo": "WHSE REC-00211",
              "SystemCreatedAt": "2024-09-10T13:40:28.2700000Z",
              "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
              "ChildLPTotalQuantities": 3.0,
              "LPLines": [
                {
                  "LineNo": 10000,
                  "ItemNo": "D0BDBD",
                  "VariantCode": "B60W225",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 2.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 20000
                },
                {
                  "LineNo": 20000,
                  "ItemNo": "D0BDBD",
                  "VariantCode": "B60W225",
                  "SerialNo": "",
                  "LotNo": "",
                  "Description": "",
                  "Quantity": 1.0,
                  "UnitofMeasure": "EA",
                  "SourceWhseLineNo": 0
                }
              ],
              "ChildLPs": []
            }
          ]
        }
      }
    ]
  },
  "Duration": "6 seconds 622 milliseconds"
}
```

#### **Explicación**
- **WarehouseInvPhysicalCount_LP**: Un array que contiene los detalles del inventario físico contado en el almacén.
  - **JournalTemplateName**: Nombre de la plantilla del diario (e.g., `"PHYSICAL I"`).
  - **JournalBatchName**: Nombre del lote del diario (e.g., `"IVAN"`).
  - **BinCode**: El bin de almacenamiento donde se encuentran los artículos (e.g., `"10C3"`).
  - **LineNo**: El número de la línea dentro del lote del diario (e.g., `10000`).
  - **ItemNo**: Número de artículo (e.g., `"1006"`).
  - **QtyPhysInventory**: Cantidad que fue contada físicamente (e.g., `1.0`).
  - **QtyCalculatedBase**: Cantidad calculada según los datos del sistema (e.g., `1.0`).
  - **LPDocumentNo**: Número de documento de la placa de licencia (e.g., `"LP-00123"`).
  - **SuperParentLP**: El número de la placa de licencia principal (e.g., `"LP-00123"`).

- **LPArray**: Un array que contiene detalles sobre las placas de licencia (LPs) y su jerarquía.
  - **SuperParentLP**: La placa de licencia principal (e.g., `"LP-00123"`).
  - **LPHierarchy**: Detalles sobre la jerarquía de la placa de licencia.
    - **LPTotalQuantities**: Cantidad total asociada a la placa de licencia (e.g., `4.0`).
    - **LPLines**: Líneas asociadas a la placa de licencia.

#### **Resumen**
El método `PreRegister_WarehouseInvPhysicalCount` procesa las discrepancias de inventario físico, transfiriendo las líneas relacionadas con LPs a un nuevo lote para revisión y devolviendo información detallada en formato JSON. Este método maneja las relaciones entre placas de licencia (LPs) y asegura la integridad del sistema de inventario al agrupar las líneas de LPs padre e hijo.

### Lógica de Implementación
1. **Validación**:
   - Se validan parámetros como la plantilla del diario, el lote y la ubicación antes de procesar.

2. **Manejo de Lotes**:
   - Se crea o se recupera el lote para gestionar las discrepancias de LPs que fueron sobrecontados o subcontados.

3. **Procesamiento de Ajustes**:
   - Se identifican las líneas en el lote original que deben transferirse al lote de revisión, asegurando que las relaciones padre-hijo de los LPs sean manejadas correctamente.

4. **Eliminación de Líneas Originales**:
   - Las líneas del lote original se eliminan una vez que se han transferido al lote de revisión.

5. **Respuesta en JSON**:
   - Se genera una estructura JSON con los detalles de las líneas contadas y no contadas, proporcionando transparencia en el proceso de revisión de inventario.