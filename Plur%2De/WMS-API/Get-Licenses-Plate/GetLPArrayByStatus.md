**ProcessMethod**: GetLPArrayByStatus

**Description**:
Method that returns the combination of Registration Headers / Registration Lines according to the **LP Status**.

**Input**:
**Parameters**: Status of the LP, the options are of the integer type as seen below
-	**IsPallet**: if the variable is true it indicates that it is Pallet, otherwise it is Single.
-	**LicensePlateStatus**:  

 -value(0; "Pre-Labeled") 
 -value(1; "Received")  
 -value(2; "Labeled")  
 -value(3; "Stored")  
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
  "ProcessMethod": "GetLPArrayByStatus",
  "Parameters": [
    {
      "IsPallet": true,
      "LicensePlateStatus":0
    }
  ]
}
```



Outputs:

```
{
  "LicensePlates": {
    "LPHeaders": [
      {
        "LicensePlatesHeaders": {
          "id": 71017598,
          "name": "PLULPHeaders",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00923),LP Document Type=CONST(Single)",
          "recordId": "PLU LP Headers: LP-00923,Single",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00923",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              }
            ]
          },
          "fieldCount": 25,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00923",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 3,
              "name": "PLUDescription",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 4,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Pre-Labeled",
              "System": false
            },
            {
              "id": 5,
              "name": "PLULocationCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 6,
              "name": "PLUZoneCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUBinCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Created By Plur-e Module.",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUUnitofMeasure",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUWarehouseEntryNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUReferenceDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 15,
              "name": "PLUReferenceNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLUDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDocumentType",
              "type": "Option",
              "value": "Whse. Journal",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 19,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 20,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 21,
              "name": "PLUItemNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 22,
              "name": "PLULPTotalQuantities",
              "type": "Decimal",
              "value": null,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{75615340-F1C1-ED11-9A88-000D3AA77A9E}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-13T22:49:03.9000000Z",
              "System": false
            },
            {
              "id": 2000000002,
              "name": "SystemCreatedBy",
              "type": "GUID",
              "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
              "System": false
            },
            {
              "id": 2000000003,
              "name": "SystemModifiedAt",
              "type": "DateTime",
              "value": "2023-03-13T22:49:03.9000000Z",
              "System": false
            },
            {
              "id": 2000000004,
              "name": "SystemModifiedBy",
              "type": "GUID",
              "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
              "System": false
            }
          ]
        }
      },
      {
        "LicensePlatesHeaders": {
          "id": 71017598,
          "name": "PLULPHeaders",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00936),LP Document Type=CONST(Single)",
          "recordId": "PLU LP Headers: LP-00936,Single",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00936",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Single",
                "System": false
              }
            ]
          },
          "fieldCount": 25,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00936",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Single",
              "System": false
            },
            {
              "id": 3,
              "name": "PLUDescription",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 4,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Pre-Labeled",
              "System": false
            },
            {
              "id": 5,
              "name": "PLULocationCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 6,
              "name": "PLUZoneCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUBinCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Created By Plur-e Module.",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUUnitofMeasure",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUWarehouseEntryNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUReferenceDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 15,
              "name": "PLUReferenceNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLUDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDocumentType",
              "type": "Option",
              "value": "Whse. Journal",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 19,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 20,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 21,
              "name": "PLUItemNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 22,
              "name": "PLULPTotalQuantities",
              "type": "Decimal",
              "value": null,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{AD197EB5-68C2-ED11-9A88-6045BD2CE534}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-14T13:04:10.5830000Z",
              "System": false
            },
            {
              "id": 2000000002,
              "name": "SystemCreatedBy",
              "type": "GUID",
              "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
              "System": false
            },
            {
              "id": 2000000003,
              "name": "SystemModifiedAt",
              "type": "DateTime",
              "value": "2023-03-14T13:04:10.5830000Z",
              "System": false
            },
            {
              "id": 2000000004,
              "name": "SystemModifiedBy",
              "type": "GUID",
              "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
              "System": false
            }
          ]
        }
      },
      {
        "LicensePlatesHeaders": {
          "id": 71017598,
          "name": "PLULPHeaders",
          "company": "CRONUS USA, Inc.",
          "position": "LP Document No.=CONST(LP-00974),LP Document Type=CONST(Pallet)",
          "recordId": "PLU LP Headers: LP-00974,Pallet",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 1,
                "name": "PLULPDocumentNo",
                "type": "Code",
                "value": "LP-00974",
                "System": false
              },
              {
                "id": 2,
                "name": "PLULPDocumentType",
                "type": "Option",
                "value": "Pallet",
                "System": false
              }
            ]
          },
          "fieldCount": 25,
          "fields": [
            {
              "id": 1,
              "name": "PLULPDocumentNo",
              "type": "Code",
              "value": "LP-00974",
              "System": false
            },
            {
              "id": 2,
              "name": "PLULPDocumentType",
              "type": "Option",
              "value": "Pallet",
              "System": false
            },
            {
              "id": 3,
              "name": "PLUDescription",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 4,
              "name": "PLULicensePlateStatus",
              "type": "Option",
              "value": "Pre-Labeled",
              "System": false
            },
            {
              "id": 5,
              "name": "PLULocationCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 6,
              "name": "PLUZoneCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "PLUBinCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 10,
              "name": "PLUWhseDocument",
              "type": "Option",
              "value": "Created By Plur-e Module.",
              "System": false
            },
            {
              "id": 11,
              "name": "PLUWhseDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 12,
              "name": "PLUUnitofMeasure",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 13,
              "name": "PLUWarehouseEntryNo",
              "type": "Integer",
              "value": null,
              "System": false
            },
            {
              "id": 14,
              "name": "PLUReferenceDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 15,
              "name": "PLUReferenceNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 16,
              "name": "PLUDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 17,
              "name": "PLUDocumentType",
              "type": "Option",
              "value": "Whse. Journal",
              "System": false
            },
            {
              "id": 18,
              "name": "PLUShipmentSrcDocument",
              "type": "Option",
              "value": " ",
              "System": false
            },
            {
              "id": 19,
              "name": "PLUShipmentSrcDocumentNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 20,
              "name": "PLUParentLPNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 21,
              "name": "PLUItemNo",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 22,
              "name": "PLULPTotalQuantities",
              "type": "Decimal",
              "value": null,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{85461750-77C2-ED11-9A88-6045BD2CE534}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-03-14T14:48:42.8970000Z",
              "System": false
            },
            {
              "id": 2000000002,
              "name": "SystemCreatedBy",
              "type": "GUID",
              "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
              "System": false
            },
            {
              "id": 2000000003,
              "name": "SystemModifiedAt",
              "type": "DateTime",
              "value": "2023-03-14T14:48:42.8970000Z",
              "System": false
            },
            {
              "id": 2000000004,
              "name": "SystemModifiedBy",
              "type": "GUID",
              "value": "{3FFD1580-3EAE-466A-8233-D5A0CC765BA8}",
              "System": false
            }
          ]
        }
      }
    ],
    "LPLines": []
  }
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


