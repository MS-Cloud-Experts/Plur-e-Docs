**ProcessMethod**: GetLicencesPlateByStatus

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
  "ProcessMethod": "GetLicencesPlateByStatus",
  "Parameters": [
    {
      "No": "WHSE REC-0000004",
      "IsPallet": true,
      "LicensePlateStatus":1
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
      "LPDocumentNo": "LP-01168",
      "DocumentLPType": "Pallet",
      "ParentLPNo": "",
      "LocationCode": "NEWWMS",
      "WhseDocumentNo": "WHSE REC-00154",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-01168),LP Document Type=CONST(Pallet),Line No.=CONST(10000)",
          "recordId": "PLU LP Lines: LP-01168,Pallet,10000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-01168",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Pallet",
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
              "value": "LP-01168",
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
              "value": "Pallet",
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
              "value": 4.0,
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
              "value": 4.0,
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
              "value": "106176",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Receipt",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE REC-00154",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Received",
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
              "value": 20000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 20000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{FF76C3FD-FCCF-ED11-A7C8-000D3A3E81B6}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-31T19:48:30.0330000Z",
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
              "value": "2023-03-31T19:48:30.2070000Z",
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
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-01168),LP Document Type=CONST(Pallet),Line No.=CONST(20000)",
          "recordId": "PLU LP Lines: LP-01168,Pallet,20000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-01168",
                "System": false
              },
              {
                "id": 3,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Pallet",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULineNo",
                "type": "Integer",
                "value": 20000,
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
              "value": "LP-01168",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 20000,
              "System": false
            },
            {
              "id": 3,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Pallet",
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
              "value": "1013",
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
              "value": 1.0,
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
              "value": 1.0,
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
              "value": "5000",
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
              "value": "1013",
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
              "value": "106176",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Receipt",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE REC-00154",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Received",
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
              "value": "{0277C3FD-FCCF-ED11-A7C8-000D3A3E81B6}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-31T19:48:31.6270000Z",
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
              "value": "2023-03-31T19:48:31.6270000Z",
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
      "LPDocumentNo": "LP-01169",
      "DocumentLPType": "Pallet",
      "ParentLPNo": "",
      "LocationCode": "NEWWMS",
      "WhseDocumentNo": "WHSE REC-00154",
      "LPLines": [
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-01157),LP Document Type=CONST(Single),Line No.=CONST(20000)",
          "recordId": "PLU LP Lines: LP-01157,Single,20000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-01157",
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
                "value": 20000,
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
              "value": "LP-01157",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 20000,
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
              "value": 3.0,
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
              "value": 3.0,
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
              "value": "106176",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Receipt",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE REC-00154",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Received",
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
              "value": 20000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 20000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{6288AA3D-CFCF-ED11-A7C9-000D3A9FD1D4}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-31T14:20:58.2830000Z",
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
              "value": "2023-03-31T14:20:58.2830000Z",
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
        {
          "id": 71017599,
          "name": "PLULPLines",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-01158),LP Document Type=CONST(Single),Line No.=CONST(20000)",
          "recordId": "PLU LP Lines: LP-01158,Single,20000",
          "primaryKey": {
            "fieldCount": 3,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-01158",
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
                "value": 20000,
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
              "value": "LP-01158",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULineNo",
              "type": "Integer",
              "value": 20000,
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
              "value": 3.0,
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
              "value": 3.0,
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
              "value": "106176",
              "System": false
            },
            {
              "id": 21,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Warehouse Receipt",
              "System": false
            },
            {
              "id": 22,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": "WHSE REC-00154",
              "System": false
            },
            {
              "id": 23,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Received",
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
              "value": 20000,
              "System": false
            },
            {
              "id": 27,
              "name": "PLUWhseLineNo",
              "type": "Integer",
              "value": 20000,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{6688AA3D-CFCF-ED11-A7C9-000D3A9FD1D4}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-31T14:20:58.4270000Z",
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
              "value": "2023-03-31T14:20:58.4270000Z",
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


