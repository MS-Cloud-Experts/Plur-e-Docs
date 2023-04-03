**ProcessMethod**: GetLicencesPlateByStatusGeneral

**Description**:
Method that returns the combination of Registration Headers / Registration Lines according to the number of the **Warehouse Receipt** with which it is filtered.

**Input**:
**Parameters**: Status of the LP, the options are of the integer type as seen below
-	**No**: Warehouse Receipt Number.
-	**IsPallet**: if the variable is true it indicates that it is Pallet, otherwise it is Single.
-	**LicensePlateStatus**:  

 -value(0; "Pre-Labeled") 
 -value(1; "Received") -> Warehouse Receipt
 -value(2; "Labeled") -> Warehouse PutAway
 -value(3; "Stored") -> Warehouse Registered PutAway
 -value(4; "Piked") 
 -value(5; "Packed") 
 -value(6; "Released") 
 -value(7; "Voided")
 -value(8; "Process") 

**Ouput**: 
-	**LicensePlates**: Contains the information of a License Plate header in **LicensePlatesHeaders** and **LicensePlatesLines** contains an array of License Plate Lines.
-	
**Example**:

Request:

```
{
  "ProcessMethod": "GetLicencesPlateByStatusGeneral",
  "Parameters": [
    {
      "No": "WHSE PUTAWAY-00174",
      "LicensePlateStatus": 2
    }
  ]
}
```



Outputs:

![image.png](/.attachments/image-5195c8c8-5405-4be5-8581-fd9d0f152dc0.png)

```
{
  "LicensePlates": [
    {
      "LPDocumentNo": "LP-00650",
      "DocumentLPType": "Single",
      "ParentLPNo": "",
      "LocationCode": "PLURE",
      "WhseDocumentNo": "WHSE PUTAWAY-00174",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00650),LP Document Type=CONST(Single),Line No.=CONST(10000)",
          "recordId": "PLU LP Lines: LP-00650,Single,10000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00650",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULineNo",
                "type": "Integer",
                "value": 10000,
                "System": false
              }
            ]
          },
          "fieldCount": 32,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00650",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 3,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 4,
              "name": "PLUType",
              "type": "Option",
              "value": "Item",
              "System": false
            },
            {
              "id": 5,
              "name": "PLUNo",
              "type": "Code",
              "value": "1906-S",
              "System": false
            },
            {
              "id": 6,
              "name": "PLUVariantCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUQuantity",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 8,
              "name": "PLUQtyperUnitofMeasure",
              "type": "Decimal",
              "value": 1.0,
              "System": false
            },
            {
              "id": 9,
              "name": "PLUQuantityBase",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUUnitofMeasureCode",
              "type": "Code",
              "value": "PCS",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUExpirationDate",
              "type": "Date",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUParentLPLineNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUStatus",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 15,
              "name": "PLUSerialNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLULotNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDescription",
              "type": "Code",
              "value": "ATHENS MOBILE PEDESTAL",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUEntryQuantity",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 19,
              "name": "PLUSourceDocument",
              "type": "Option",
              "value": "Purchase Order",
              "System": false
            },
            {
              "id": 20,
              "name": "PLUSourceDocumentNo",
              "type": "Code",
              "value": "106136",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Putway",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE PUTAWAY-00174",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Labeled",
              "System": false
            },
            {
              "id": 24,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 25,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 26,
              "name": "PLUSourceLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{BBBEEB85-87BE-ED11-9A88-000D3A969B1E}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-09T14:34:41.1900000Z",
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
              "value": "2023-03-09T14:35:19.6030000Z",
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
        }
      ]
    },
    {
      "LPDocumentNo": "LP-00651",
      "DocumentLPType": "Single",
      "ParentLPNo": "",
      "LocationCode": "PLURE",
      "WhseDocumentNo": "WHSE PUTAWAY-00174",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00651),LP Document Type=CONST(Single),Line No.=CONST(10000)",
          "recordId": "PLU LP Lines: LP-00651,Single,10000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00651",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULineNo",
                "type": "Integer",
                "value": 10000,
                "System": false
              }
            ]
          },
          "fieldCount": 32,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00651",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 3,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 4,
              "name": "PLUType",
              "type": "Option",
              "value": "Item",
              "System": false
            },
            {
              "id": 5,
              "name": "PLUNo",
              "type": "Code",
              "value": "1906-S",
              "System": false
            },
            {
              "id": 6,
              "name": "PLUVariantCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUQuantity",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 8,
              "name": "PLUQtyperUnitofMeasure",
              "type": "Decimal",
              "value": 1.0,
              "System": false
            },
            {
              "id": 9,
              "name": "PLUQuantityBase",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUUnitofMeasureCode",
              "type": "Code",
              "value": "PCS",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUExpirationDate",
              "type": "Date",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUParentLPLineNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUStatus",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 15,
              "name": "PLUSerialNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLULotNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDescription",
              "type": "Code",
              "value": "ATHENS MOBILE PEDESTAL",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUEntryQuantity",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 19,
              "name": "PLUSourceDocument",
              "type": "Option",
              "value": "Purchase Order",
              "System": false
            },
            {
              "id": 20,
              "name": "PLUSourceDocumentNo",
              "type": "Code",
              "value": "106136",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Putway",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE PUTAWAY-00174",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Labeled",
              "System": false
            },
            {
              "id": 24,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 25,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 26,
              "name": "PLUSourceLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{BFBEEB85-87BE-ED11-9A88-000D3A969B1E}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-09T14:34:41.2700000Z",
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
              "value": "2023-03-09T14:35:19.6200000Z",
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
        }
      ]
    },
    {
      "LPDocumentNo": "LP-00652",
      "DocumentLPType": "Single",
      "ParentLPNo": "",
      "LocationCode": "PLURE",
      "WhseDocumentNo": "WHSE PUTAWAY-00174",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00652),LP Document Type=CONST(Single),Line No.=CONST(10000)",
          "recordId": "PLU LP Lines: LP-00652,Single,10000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00652",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULineNo",
                "type": "Integer",
                "value": 10000,
                "System": false
              }
            ]
          },
          "fieldCount": 32,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00652",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 3,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 4,
              "name": "PLUType",
              "type": "Option",
              "value": "Item",
              "System": false
            },
            {
              "id": 5,
              "name": "PLUNo",
              "type": "Code",
              "value": "1906-S",
              "System": false
            },
            {
              "id": 6,
              "name": "PLUVariantCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUQuantity",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 8,
              "name": "PLUQtyperUnitofMeasure",
              "type": "Decimal",
              "value": 1.0,
              "System": false
            },
            {
              "id": 9,
              "name": "PLUQuantityBase",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUUnitofMeasureCode",
              "type": "Code",
              "value": "PCS",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUExpirationDate",
              "type": "Date",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUParentLPLineNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUStatus",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 15,
              "name": "PLUSerialNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLULotNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDescription",
              "type": "Code",
              "value": "ATHENS MOBILE PEDESTAL",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUEntryQuantity",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 19,
              "name": "PLUSourceDocument",
              "type": "Option",
              "value": "Purchase Order",
              "System": false
            },
            {
              "id": 20,
              "name": "PLUSourceDocumentNo",
              "type": "Code",
              "value": "106136",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Putway",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE PUTAWAY-00174",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Labeled",
              "System": false
            },
            {
              "id": 24,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 25,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 26,
              "name": "PLUSourceLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{C3BEEB85-87BE-ED11-9A88-000D3A969B1E}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-09T14:34:41.2700000Z",
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
              "value": "2023-03-09T14:35:19.6200000Z",
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
        }
      ]
    },
    {
      "LPDocumentNo": "LP-00653",
      "DocumentLPType": "Single",
      "ParentLPNo": "",
      "LocationCode": "PLURE",
      "WhseDocumentNo": "WHSE PUTAWAY-00174",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00653),LP Document Type=CONST(Single),Line No.=CONST(10000)",
          "recordId": "PLU LP Lines: LP-00653,Single,10000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00653",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULineNo",
                "type": "Integer",
                "value": 10000,
                "System": false
              }
            ]
          },
          "fieldCount": 32,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00653",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 3,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 4,
              "name": "PLUType",
              "type": "Option",
              "value": "Item",
              "System": false
            },
            {
              "id": 5,
              "name": "PLUNo",
              "type": "Code",
              "value": "1906-S",
              "System": false
            },
            {
              "id": 6,
              "name": "PLUVariantCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUQuantity",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 8,
              "name": "PLUQtyperUnitofMeasure",
              "type": "Decimal",
              "value": 1.0,
              "System": false
            },
            {
              "id": 9,
              "name": "PLUQuantityBase",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUUnitofMeasureCode",
              "type": "Code",
              "value": "PCS",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUExpirationDate",
              "type": "Date",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUParentLPLineNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUStatus",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 15,
              "name": "PLUSerialNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLULotNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDescription",
              "type": "Code",
              "value": "ATHENS MOBILE PEDESTAL",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUEntryQuantity",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 19,
              "name": "PLUSourceDocument",
              "type": "Option",
              "value": "Purchase Order",
              "System": false
            },
            {
              "id": 20,
              "name": "PLUSourceDocumentNo",
              "type": "Code",
              "value": "106136",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Putway",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE PUTAWAY-00174",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Labeled",
              "System": false
            },
            {
              "id": 24,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 25,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 26,
              "name": "PLUSourceLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{C7BEEB85-87BE-ED11-9A88-000D3A969B1E}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-09T14:34:41.2830000Z",
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
              "value": "2023-03-09T14:35:19.6370000Z",
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
        }
      ]
    },
    {
      "LPDocumentNo": "LP-00654",
      "DocumentLPType": "Single",
      "ParentLPNo": "",
      "LocationCode": "PLURE",
      "WhseDocumentNo": "WHSE PUTAWAY-00174",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00654),LP Document Type=CONST(Single),Line No.=CONST(10000)",
          "recordId": "PLU LP Lines: LP-00654,Single,10000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00654",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULineNo",
                "type": "Integer",
                "value": 10000,
                "System": false
              }
            ]
          },
          "fieldCount": 32,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00654",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 3,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 4,
              "name": "PLUType",
              "type": "Option",
              "value": "Item",
              "System": false
            },
            {
              "id": 5,
              "name": "PLUNo",
              "type": "Code",
              "value": "1906-S",
              "System": false
            },
            {
              "id": 6,
              "name": "PLUVariantCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUQuantity",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 8,
              "name": "PLUQtyperUnitofMeasure",
              "type": "Decimal",
              "value": 1.0,
              "System": false
            },
            {
              "id": 9,
              "name": "PLUQuantityBase",
              "type": "Decimal",
              "value": 2.0,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUUnitofMeasureCode",
              "type": "Code",
              "value": "PCS",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUExpirationDate",
              "type": "Date",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUParentLPLineNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUStatus",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 15,
              "name": "PLUSerialNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLULotNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDescription",
              "type": "Code",
              "value": "ATHENS MOBILE PEDESTAL",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUEntryQuantity",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 19,
              "name": "PLUSourceDocument",
              "type": "Option",
              "value": "Purchase Order",
              "System": false
            },
            {
              "id": 20,
              "name": "PLUSourceDocumentNo",
              "type": "Code",
              "value": "106136",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Putway",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE PUTAWAY-00174",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Labeled",
              "System": false
            },
            {
              "id": 24,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 25,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 26,
              "name": "PLUSourceLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 10000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{CBBEEB85-87BE-ED11-9A88-000D3A969B1E}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-09T14:34:41.2830000Z",
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
              "value": "2023-03-09T14:35:19.6370000Z",
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
        }
      ]
    }
  ]
}
```
**Error**:
```
{
  "Error": {
    "Code": "Not found",
    "Message": "The Licences Plate List is Empty"
  }
}
```


