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
      "position": "Type=CONST(Put-away),No.=CONST(10112)",
      "recordId": "Warehouse Activity Header: Put-away,10112",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "Type",
            "type": "Option",
            "value": "Put-away",
            "System": "false"
          },
          {
            "id": 2,
            "name": "No",
            "type": "Code",
            "value": 10112,
            "System": "false"
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
          "System": "false"
        },
        {
          "id": 2,
          "name": "No",
          "type": "Code",
          "value": 10112,
          "System": "false"
        },
        {
          "id": 3,
          "name": "LocationCode",
          "type": "Code",
          "value": "BBB",
          "System": "false"
        },
        {
          "id": 4,
          "name": "AssignedUserID",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 5,
          "name": "AssignmentDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 6,
          "name": "AssignmentTime",
          "type": "Time",
          "value": null,
          "System": "false"
        },
        {
          "id": 7,
          "name": "SortingMethod",
          "type": "Option",
          "value": " ",
          "System": "false"
        },
        {
          "id": 9,
          "name": "NoSeries",
          "type": "Code",
          "value": "PICK",
          "System": "false"
        },
        {
          "id": 10,
          "name": "Comment",
          "type": "Boolean",
          "value": "false",
          "System": "false"
        },
        {
          "id": 12,
          "name": "NoPrinted",
          "type": "Integer",
          "value": null,
          "System": "false"
        },
        {
          "id": 13,
          "name": "NoofLines",
          "type": "Integer",
          "value": 6,
          "System": "false"
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 61,
          "name": "RegisteringNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 62,
          "name": "LastRegisteringNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 63,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": "PICK",
          "System": "false"
        },
        {
          "id": 7303,
          "name": "DateofLastPrinting",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 7304,
          "name": "TimeofLastPrinting",
          "type": "Time",
          "value": null,
          "System": "false"
        },
        {
          "id": 7305,
          "name": "BreakbulkFilter",
          "type": "Boolean",
          "value": "false",
          "System": "false"
        },
        {
          "id": 7306,
          "name": "SourceNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 7307,
          "name": "SourceDocument",
          "type": "Option",
          "value": " ",
          "System": "false"
        },
        {
          "id": 7308,
          "name": "SourceType",
          "type": "Integer",
          "value": null,
          "System": "false"
        },
        {
          "id": 7309,
          "name": "SourceSubtype",
          "type": "Option",
          "value": 0,
          "System": "false"
        },
        {
          "id": 7310,
          "name": "DestinationType",
          "type": "Option",
          "value": " ",
          "System": "false"
        },
        {
          "id": 7311,
          "name": "DestinationNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 7312,
          "name": "ExternalDocumentNo",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 7313,
          "name": "ExpectedReceiptDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 7314,
          "name": "ShipmentDate",
          "type": "Date",
          "value": null,
          "System": "false"
        },
        {
          "id": 7315,
          "name": "ExternalDocumentNo2",
          "type": "Code",
          "value": null,
          "System": "false"
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{52D2F71F-5D96-EC11-80F2-000D3A74F81B}",
          "System": "false"
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-25T17:05:26.8930000Z",
          "System": "false"
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": "false"
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-02-25T17:05:26.8930000Z",
          "System": "false"
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": "false"
        }
      ]
    },
    "WarehousePutAwayLines": [
      {
        "id": 5767,
        "name": "WarehouseActivityLine",
        "company": "CRONUS USA, Inc.",
        "position": "Activity Type=CONST(Put-away),No.=CONST(10112),Line No.=CONST(10000)",
        "recordId": "Warehouse Activity Line: Put-away,10112,10000",
        "primaryKey": {
          "fieldCount": 3,
          "fields": [
            {
              "id": 1,
              "name": "ActivityType",
              "type": "Option",
              "value": "Put-away",
              "System": "false"
            },
            {
              "id": 2,
              "name": "No",
              "type": "Code",
              "value": 10112,
              "System": "false"
            },
            {
              "id": 3,
              "name": "LineNo",
              "type": "Integer",
              "value": 10000,
              "System": "false"
            }
          ]
        },
        "fieldCount": 67,
        "fields": [
          {
            "id": 1,
            "name": "ActivityType",
            "type": "Option",
            "value": "Put-away",
            "System": "false"
          },
          {
            "id": 2,
            "name": "No",
            "type": "Code",
            "value": 10112,
            "System": "false"
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 10000,
            "System": "false"
          },
          {
            "id": 4,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": "false"
          },
          {
            "id": 5,
            "name": "SourceSubtype",
            "type": "Option",
            "value": 1,
            "System": "false"
          },
          {
            "id": 6,
            "name": "SourceNo",
            "type": "Code",
            "value": 106041,
            "System": "false"
          },
          {
            "id": 7,
            "name": "SourceLineNo",
            "type": "Integer",
            "value": 10000,
            "System": "false"
          },
          {
            "id": 8,
            "name": "SourceSublineNo",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 9,
            "name": "SourceDocument",
            "type": "Option",
            "value": "Purchase Order",
            "System": "false"
          },
          {
            "id": 11,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": "false"
          },
          {
            "id": 12,
            "name": "ShelfNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 13,
            "name": "SortingSequenceNo",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 14,
            "name": "ItemNo",
            "type": "Code",
            "value": 100,
            "System": "false"
          },
          {
            "id": 15,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 16,
            "name": "UnitofMeasureCode",
            "type": "Code",
            "value": "PCS",
            "System": "false"
          },
          {
            "id": 17,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": "false"
          },
          {
            "id": 18,
            "name": "Description",
            "type": "Text",
            "value": "TEST",
            "System": "false"
          },
          {
            "id": 19,
            "name": "Description2",
            "type": "Text",
            "value": null,
            "System": "false"
          },
          {
            "id": 20,
            "name": "Quantity",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 21,
            "name": "Qty(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 24,
            "name": "QtyOutstanding",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 25,
            "name": "QtyOutstanding(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 26,
            "name": "QtytoHandle",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 27,
            "name": "QtytoHandle(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 28,
            "name": "QtyHandled",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 29,
            "name": "QtyHandled(Base)",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 31,
            "name": "ShippingAdvice",
            "type": "Option",
            "value": "Partial",
            "System": "false"
          },
          {
            "id": 34,
            "name": "DueDate",
            "type": "Date",
            "value": "2022-02-04",
            "System": "false"
          },
          {
            "id": 39,
            "name": "DestinationType",
            "type": "Option",
            "value": " ",
            "System": "false"
          },
          {
            "id": 40,
            "name": "DestinationNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 42,
            "name": "ShippingAgentCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 43,
            "name": "ShippingAgentServiceCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 44,
            "name": "ShipmentMethodCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 47,
            "name": "StartingDate",
            "type": "Date",
            "value": "2022-02-04",
            "System": "false"
          },
          {
            "id": 50,
            "name": "QtyRoundingPrecision",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 51,
            "name": "QtyRoundingPrecision(Base)",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 900,
            "name": "AssembletoOrder",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 901,
            "name": "ATOComponent",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 6500,
            "name": "SerialNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 6501,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 6502,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": "false"
          },
          {
            "id": 6503,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": "false"
          },
          {
            "id": 6504,
            "name": "SerialNoBlocked",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 6505,
            "name": "LotNoBlocked",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 7300,
            "name": "BinCode",
            "type": "Code",
            "value": "REC",
            "System": "false"
          },
          {
            "id": 7301,
            "name": "ZoneCode",
            "type": "Code",
            "value": "REC",
            "System": "false"
          },
          {
            "id": 7305,
            "name": "ActionType",
            "type": "Option",
            "value": "Take",
            "System": "false"
          },
          {
            "id": 7306,
            "name": "WhseDocumentType",
            "type": "Option",
            "value": "Receipt",
            "System": "false"
          },
          {
            "id": 7307,
            "name": "WhseDocumentNo",
            "type": "Code",
            "value": "PTWHRCT01156",
            "System": "false"
          },
          {
            "id": 7308,
            "name": "WhseDocumentLineNo",
            "type": "Integer",
            "value": 10000,
            "System": "false"
          },
          {
            "id": 7309,
            "name": "BinRanking",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 7310,
            "name": "Cubage",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 7311,
            "name": "Weight",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 7312,
            "name": "SpecialEquipmentCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 7313,
            "name": "BinTypeCode",
            "type": "Code",
            "value": "REC",
            "System": "false"
          },
          {
            "id": 7314,
            "name": "BreakbulkNo",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 7315,
            "name": "OriginalBreakbulk",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 7316,
            "name": "Breakbulk",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 7317,
            "name": "CrossDockInformation",
            "type": "Option",
            "value": " ",
            "System": "false"
          },
          {
            "id": 7318,
            "name": "Dedicated",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 71017575,
            "name": "PLUNoLPCreated",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{54D2F71F-5D96-EC11-80F2-000D3A74F81B}",
            "System": "false"
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2022-02-25T17:05:26.9870000Z",
            "System": "false"
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": "false"
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2022-02-25T17:05:26.9870000Z",
            "System": "false"
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": "false"
          }
        ]
      },
      {
        "id": 5767,
        "name": "WarehouseActivityLine",
        "company": "CRONUS USA, Inc.",
        "position": "Activity Type=CONST(Put-away),No.=CONST(10112),Line No.=CONST(20000)",
        "recordId": "Warehouse Activity Line: Put-away,10112,20000",
        "primaryKey": {
          "fieldCount": 3,
          "fields": [
            {
              "id": 1,
              "name": "ActivityType",
              "type": "Option",
              "value": "Put-away",
              "System": "false"
            },
            {
              "id": 2,
              "name": "No",
              "type": "Code",
              "value": 10112,
              "System": "false"
            },
            {
              "id": 3,
              "name": "LineNo",
              "type": "Integer",
              "value": 20000,
              "System": "false"
            }
          ]
        },
        "fieldCount": 67,
        "fields": [
          {
            "id": 1,
            "name": "ActivityType",
            "type": "Option",
            "value": "Put-away",
            "System": "false"
          },
          {
            "id": 2,
            "name": "No",
            "type": "Code",
            "value": 10112,
            "System": "false"
          },
          {
            "id": 3,
            "name": "LineNo",
            "type": "Integer",
            "value": 20000,
            "System": "false"
          },
          {
            "id": 4,
            "name": "SourceType",
            "type": "Integer",
            "value": 39,
            "System": "false"
          },
          {
            "id": 5,
            "name": "SourceSubtype",
            "type": "Option",
            "value": 1,
            "System": "false"
          },
          {
            "id": 6,
            "name": "SourceNo",
            "type": "Code",
            "value": 106041,
            "System": "false"
          },
          {
            "id": 7,
            "name": "SourceLineNo",
            "type": "Integer",
            "value": 10000,
            "System": "false"
          },
          {
            "id": 8,
            "name": "SourceSublineNo",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 9,
            "name": "SourceDocument",
            "type": "Option",
            "value": "Purchase Order",
            "System": "false"
          },
          {
            "id": 11,
            "name": "LocationCode",
            "type": "Code",
            "value": "BBB",
            "System": "false"
          },
          {
            "id": 12,
            "name": "ShelfNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 13,
            "name": "SortingSequenceNo",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 14,
            "name": "ItemNo",
            "type": "Code",
            "value": 100,
            "System": "false"
          },
          {
            "id": 15,
            "name": "VariantCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 16,
            "name": "UnitofMeasureCode",
            "type": "Code",
            "value": "PCS",
            "System": "false"
          },
          {
            "id": 17,
            "name": "QtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": "false"
          },
          {
            "id": 18,
            "name": "Description",
            "type": "Text",
            "value": "TEST",
            "System": "false"
          },
          {
            "id": 19,
            "name": "Description2",
            "type": "Text",
            "value": null,
            "System": "false"
          },
          {
            "id": 20,
            "name": "Quantity",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 21,
            "name": "Qty(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 24,
            "name": "QtyOutstanding",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 25,
            "name": "QtyOutstanding(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 26,
            "name": "QtytoHandle",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 27,
            "name": "QtytoHandle(Base)",
            "type": "Decimal",
            "value": 10.0,
            "System": "false"
          },
          {
            "id": 28,
            "name": "QtyHandled",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 29,
            "name": "QtyHandled(Base)",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 31,
            "name": "ShippingAdvice",
            "type": "Option",
            "value": "Partial",
            "System": "false"
          },
          {
            "id": 34,
            "name": "DueDate",
            "type": "Date",
            "value": "2022-02-04",
            "System": "false"
          },
          {
            "id": 39,
            "name": "DestinationType",
            "type": "Option",
            "value": " ",
            "System": "false"
          },
          {
            "id": 40,
            "name": "DestinationNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 42,
            "name": "ShippingAgentCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 43,
            "name": "ShippingAgentServiceCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 44,
            "name": "ShipmentMethodCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 47,
            "name": "StartingDate",
            "type": "Date",
            "value": "2022-02-04",
            "System": "false"
          },
          {
            "id": 50,
            "name": "QtyRoundingPrecision",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 51,
            "name": "QtyRoundingPrecision(Base)",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 900,
            "name": "AssembletoOrder",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 901,
            "name": "ATOComponent",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 6500,
            "name": "SerialNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 6501,
            "name": "LotNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 6502,
            "name": "WarrantyDate",
            "type": "Date",
            "value": null,
            "System": "false"
          },
          {
            "id": 6503,
            "name": "ExpirationDate",
            "type": "Date",
            "value": null,
            "System": "false"
          },
          {
            "id": 6504,
            "name": "SerialNoBlocked",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 6505,
            "name": "LotNoBlocked",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 6515,
            "name": "PackageNo",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 7300,
            "name": "BinCode",
            "type": "Code",
            "value": "STO1",
            "System": "false"
          },
          {
            "id": 7301,
            "name": "ZoneCode",
            "type": "Code",
            "value": "STO",
            "System": "false"
          },
          {
            "id": 7305,
            "name": "ActionType",
            "type": "Option",
            "value": "Place",
            "System": "false"
          },
          {
            "id": 7306,
            "name": "WhseDocumentType",
            "type": "Option",
            "value": "Receipt",
            "System": "false"
          },
          {
            "id": 7307,
            "name": "WhseDocumentNo",
            "type": "Code",
            "value": "PTWHRCT01156",
            "System": "false"
          },
          {
            "id": 7308,
            "name": "WhseDocumentLineNo",
            "type": "Integer",
            "value": 10000,
            "System": "false"
          },
          {
            "id": 7309,
            "name": "BinRanking",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 7310,
            "name": "Cubage",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 7311,
            "name": "Weight",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 7312,
            "name": "SpecialEquipmentCode",
            "type": "Code",
            "value": null,
            "System": "false"
          },
          {
            "id": 7313,
            "name": "BinTypeCode",
            "type": "Code",
            "value": "STORAGE",
            "System": "false"
          },
          {
            "id": 7314,
            "name": "BreakbulkNo",
            "type": "Integer",
            "value": null,
            "System": "false"
          },
          {
            "id": 7315,
            "name": "OriginalBreakbulk",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 7316,
            "name": "Breakbulk",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 7317,
            "name": "CrossDockInformation",
            "type": "Option",
            "value": " ",
            "System": "false"
          },
          {
            "id": 7318,
            "name": "Dedicated",
            "type": "Boolean",
            "value": "false",
            "System": "false"
          },
          {
            "id": 71017575,
            "name": "PLUNoLPCreated",
            "type": "Decimal",
            "value": null,
            "System": "false"
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{53D2F71F-5D96-EC11-80F2-000D3A74F81B}",
            "System": "false"
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2022-02-25T17:05:26.9400000Z",
            "System": "false"
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": "false"
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2022-02-25T17:05:26.9400000Z",
            "System": "false"
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": "false"
          }
        ]
      }
    ]
  }
}
```

**Errors**:

`"{"Error":" The Warehouse Put-Away does not exist"}`"



