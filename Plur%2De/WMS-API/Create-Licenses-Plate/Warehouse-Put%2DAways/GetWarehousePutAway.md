**ProcessMethod**: GetWarehousePutAway

**Description**:
This method returns the elements of the table "Warehouse Activity Header" filtered so that only "Put-Away" is visible. In this case, the filtered record is brought in the "No" field. returning the "Warehouse Activity Header" and the "Warehouse Activity Line" in JSON format.

Note: There is a table called " Warehouse Activity Header" which contains all registered Put-Aways and Pick, changing only the Type for differences between one or the other.

**Input**:
**Parameters**: 
-	**No**: Allows you to bring a single Warehouse Activity Header. 

**Ouput**:  

-	**WarehousePutAways**: Contains a Registered `WarehousePutAwayHeader` and an array of lines expressed in the key: `WarehouseActivityLine`.
-	
   Note: Each WarehouseActivityLine array must contain 2 lines.

The first must have the **Action Type**: **Take** and the second must be **Place**.

This tells us that the first one takes the Item from the `Origin Bin` and stores it in the second line that would represent the `Destination Bin`.

**Example**:

**WarehousePutAwayHeader:**
![image.png](/.attachments/image-e64a6139-5636-4d83-9337-1d3ec743901f.png)

**WarehouseActivityLine:**
![image.png](/.attachments/image-04c42856-a2bc-4fc0-a83d-676c995ecfc0.png)

**Request**:

    `"jsonRequest":"{\"ProcessMethod\":\"GetWarehousePutAway\",\"Parameters\":[{\"No\":\"10112\"}]}"`

Outputs:

```
{
  "WarehousePutAways": {
    "WarehousePutAwayHeader": {
      "id": 5766,
      "name": "WarehouseActivityHeader",
      "company": "CRONUS USA, Inc.",
      "position": "Type=CONST(Put-away),No.=CONST(WHSE PUTAWAY-00169)",
      "recordId": "Warehouse Activity Header: Put-away,WHSE PUTAWAY-00169",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "Type",
            "type": "Option",
            "value": "Put-away",
            "System": false
          },
          {
            "id": 2,
            "name": "No",
            "type": "Code",
            "value": "WHSE PUTAWAY-00169",
            "System": false
          }
        ]
      },
      "fieldCount": 33,
      "fields": [
        {
          "id": 1,
          "name": "Type",
          "type": "Option",
          "value": "Put-away",
          "System": false
        },
        {
          "id": 2,
          "name": "No",
          "type": "Code",
          "value": "WHSE PUTAWAY-00169",
          "System": false
        },
        {
          "id": 3,
          "name": "LocationCode",
          "type": "Code",
          "value": "PLURE",
          "System": false
        },
        {
          "id": 4,
          "name": "AssignedUserID",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5,
          "name": "AssignmentDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 6,
          "name": "AssignmentTime",
          "type": "Time",
          "value": null,
          "System": false
        },
        {
          "id": 7,
          "name": "SortingMethod",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 9,
          "name": "NoSeries",
          "type": "Code",
          "value": "WHSE PUTAWAY",
          "System": false
        },
        {
          "id": 10,
          "name": "Comment",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 12,
          "name": "NoPrinted",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 13,
          "name": "NoofLines",
          "type": "Integer",
          "value": 16,
          "System": false
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 61,
          "name": "RegisteringNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 62,
          "name": "LastRegisteringNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 63,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": "REG PUTAWAY",
          "System": false
        },
        {
          "id": 7303,
          "name": "DateofLastPrinting",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 7304,
          "name": "TimeofLastPrinting",
          "type": "Time",
          "value": null,
          "System": false
        },
        {
          "id": 7305,
          "name": "BreakbulkFilter",
          "type": "Boolean",
          "value": false,
          "System": false
        },
        {
          "id": 7306,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7307,
          "name": "SourceDocument",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 7308,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": false
        },
        {
          "id": 7309,
          "name": "SourceSubtype",
          "type": "Option",
          "value": "0",
          "System": false
        },
        {
          "id": 7310,
          "name": "DestinationType",
          "type": "Option",
          "value": " ",
          "System": false
        },
        {
          "id": 7311,
          "name": "DestinationNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7312,
          "name": "ExternalDocumentNo",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7313,
          "name": "ExpectedReceiptDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 7314,
          "name": "ShipmentDate",
          "type": "Date",
          "value": null,
          "System": false
        },
        {
          "id": 7315,
          "name": "ExternalDocumentNo2",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{50A28802-D1BD-ED11-9A88-6045BD2C94D4}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2023-03-08T16:48:15.8430000Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2023-03-08T16:48:15.8430000Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{D88F4C11-86DD-4E04-BB28-D250592C231E}",
          "System": false
        }
      ]
    },
    "WarehousePutAwayLines": [
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "10000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "20000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00628",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "30000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "40000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00628",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "50000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "60000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00628",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "70000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "80000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00628",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "90000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "100000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00630",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "110000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "120000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00630",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "130000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "140000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00631",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "150000",
        "ZoneCode": "REC",
        "LocationCode": "PLURE",
        "BinCode": "REC-1",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      },
      {
        "No": "WHSE PUTAWAY-00169",
        "ItemNo": "1013",
        "VariantCode": "",
        "LineNo": "160000",
        "ZoneCode": "STO",
        "LocationCode": "PLURE",
        "BinCode": "",
        "Quantity": 1.0,
        "UnitofMeasureCode": "PCS",
        "QtyperUnitofMeasure": 1.0,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceNo": "106125",
        "SourceLineNo": 10000,
        "Managed_by_PlurE": true,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SNALLWH",
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "LP-00631",
        "PLULPPalletChildsasLP": "",
        "PLULPPalletChildasItems": ""
      }
    ]
  }
}
```

**Errors**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Put-Away does not exist""
  }
}
```

