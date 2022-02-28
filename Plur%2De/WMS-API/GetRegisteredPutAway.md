**ProcessMethod**: GetRegisteredPutAway

**Description**:
This method returns the elements of the table "**Registered Whse. Activity Hdr.**" filtered so that only "**Registered Put-Away**" is visible. In this case, the filtered record is brought in the "**No**" field. returning the "**Registered Whse. Activity Hdr**" and the "R**egistered Whse. Activity Line**" in JSON format.

Note: There is a table called "**Registered Whse. Activity Hdr.**" which contains all registered **Put-Aways** and **Pick-Ups**, changing only the Type for differences between one or the other.

**Input**:
**Parameters**: 
-	**No**: Allows you to bring a single Registered Whse Activity Hdr. 

**Ouput**:  

-	**RegisteredWhseActivity**: Contains a **RegisteredWhseActivityHdr** and an array of lines expressed in the key: **RegisteredWhseActivityLine**.
-	
   **Note**: Each RegisteredWhseActivityLine array must contain 2 lines.

The first must have the Action Type: **Take** and the second must be **Place**.

This tells us that the first one takes the Item from the **Origin Bin** and stores it in the second line that would represent the **Destination Bin**.

**Example**:

**Registered WhseActivityHdr:**
![image.png](/.attachments/image-630904a0-db24-4f9a-9dff-26d3b9290f35.png)

**RegisteredWhseActivityLine:**
![image.png](/.attachments/image-df634b8c-8f92-4037-bef4-c5a513f4a1f0.png)

**Request:**
`"jsonRequest":"{"ProcessMethod":"GetRegisteredPutAway","Parameters":[{"No":"10111"}]}"`

**Outputs**:

 
```
{
  "RegisteredWhseActivity": {
    "RegisteredWhseActivityHdr": {
      "id": 5772,
      "name": "RegisteredWhseActivityHdr",
      "company": "CRONUS USA, Inc.",
      "position": "Type=CONST(Put-away),No.=CONST(10111)",
      "recordId": "Registered Whse. Activity Hdr.: Put-away,10111",
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
            "value": 10111,
            "System": "false"
          }
        ]
      },
      "fieldCount": 17,
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
          "value": 10111,
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
          "id": 8,
          "name": "RegisteringDate",
          "type": "Date",
          "value": "2022-02-25",
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
          "id": 11,
          "name": "WhseActivityNo",
          "type": "Code",
          "value": 10110,
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
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{665F4DE5-5B96-EC11-80F2-000D3A74F81B}",
          "System": "false"
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-25T16:56:38.5030000Z",
          "System": "false"
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
          "System": "false"
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-02-25T16:56:38.5030000Z",
          "System": "false"
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
          "System": "false"
        }
      ]
    },
    "RegisteredWhseActivityLine": [
      {
        "id": 5773,
        "name": "RegisteredWhseActivityLine",
        "company": "CRONUS USA, Inc.",
        "position": "Activity Type=CONST(Put-away),No.=CONST(10111),Line No.=CONST(10000)",
        "recordId": "Registered Whse. Activity Line: Put-away,10111,10000",
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
              "value": 10111,
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
        "fieldCount": 49,
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
            "value": 10111,
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
            "value": 106039,
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
            "value": "100A",
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
            "value": "100A",
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
            "id": 41,
            "name": "WhseActivityNo",
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
            "value": "PTWHRCT01155",
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
            "value": "{695F4DE5-5B96-EC11-80F2-000D3A74F81B}",
            "System": "false"
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2022-02-25T16:56:38.5500000Z",
            "System": "false"
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
            "System": "false"
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2022-02-25T16:56:38.5500000Z",
            "System": "false"
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
            "System": "false"
          }
        ]
      },
      {
        "id": 5773,
        "name": "RegisteredWhseActivityLine",
        "company": "CRONUS USA, Inc.",
        "position": "Activity Type=CONST(Put-away),No.=CONST(10111),Line No.=CONST(20000)",
        "recordId": "Registered Whse. Activity Line: Put-away,10111,20000",
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
              "value": 10111,
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
        "fieldCount": 49,
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
            "value": 10111,
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
            "value": 106039,
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
            "value": "100A",
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
            "value": "100A",
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
            "id": 41,
            "name": "WhseActivityNo",
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
            "value": "STO2",
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
            "value": "PTWHRCT01155",
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
            "value": "{6B5F4DE5-5B96-EC11-80F2-000D3A74F81B}",
            "System": "false"
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2022-02-25T16:56:38.5830000Z",
            "System": "false"
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
            "System": "false"
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2022-02-25T16:56:38.5830000Z",
            "System": "false"
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{91087AD1-8546-4750-A87C-5445D04F7C7A}",
            "System": "false"
          }
        ]
      }
    ]
  }
}
```
Errors:

`"{"Error":"The Registered Whse. Activity Hdr. not exist"}"`

