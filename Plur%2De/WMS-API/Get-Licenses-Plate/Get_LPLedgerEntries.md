**ProcessMethod**: Get_LPLedgerEntries

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
  "ProcessMethod": "Get_LPLedgerEntries",
  "Parameters": [
    {
      "No": "LP-0000779"
    }
  ]
}
```



Outputs:

![image.png](/.attachments/image-5195c8c8-5405-4be5-8581-fd9d0f152dc0.png)

```
{
  "LicensePlates": {
    "LicensePlatesHeaders": {
      "id": 71017590,
      "name": "PLULicensePlatesHeaders",
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(LP000205)",
      "recordId": "PLU License Plates Headers: LP000205",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 1,
            "name": "PLUNo",
            "type": "Code",
            "value": "LP000205",
            "System": false
          }
        ]
      },
      "fieldCount": 15,
      "fields": [
        {
          "id": 1,
          "name": "PLUNo",
          "type": "Code",
          "value": "LP000205",
          "System": false
        },
        {
          "id": 2,
          "name": "PLUDescription",
          "type": "Text",
          "value": "SYDNEY Swivel Chair, green",
          "System": false
        },
        {
          "id": 3,
          "name": "PLULicensePlateStatus",
          "type": "Option",
          "value": "Labeled",
          "System": false
        },
        {
          "id": 4,
          "name": "PLULocationCode",
          "type": "Code",
          "value": "BBB",
          "System": false
        },
        {
          "id": 5,
          "name": "PLUBinCode",
          "type": "Code",
          "value": "STO2",
          "System": false
        },
        {
          "id": 6,
          "name": "PLUSourceDocument",
          "type": "Option",
          "value": "Purchase Order",
          "System": false
        },
        {
          "id": 7,
          "name": "PLUSourceDocumentNo",
          "type": "Code",
          "value": "106031",
          "System": false
        },
        {
          "id": 8,
          "name": "PLUDocument",
          "type": "Option",
          "value": "Warehouse Putway",
          "System": false
        },
        {
          "id": 9,
          "name": "PLUDocumentNo",
          "type": "Code",
          "value": "10090",
          "System": false
        },
        {
          "id": 10,
          "name": "PLUUnitofMeasure",
          "type": "Code",
          "value": "PACK",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{53E5ED53-0C91-EC11-B85A-000D3A74F81B}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-18T22:44:29.197Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-02-18T22:45:23.943Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": false
        }
      ]
    },
    "LicensePlatesLines": [
      {
        "id": 71017591,
        "name": "PLULicensePlatesLines",
        "company": "CRONUS USA, Inc.",
        "position": "No.=CONST(LP000205),Line No.=CONST(20000)",
        "recordId": "PLU License Plates Lines: LP000205,20000",
        "primaryKey": {
          "fieldCount": 2,
          "fields": [
            {
              "id": 1,
              "name": "PLUNo",
              "type": "Code",
              "value": "LP000205",
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
        "fieldCount": 26,
        "fields": [
          {
            "id": 1,
            "name": "PLUNo",
            "type": "Code",
            "value": "LP000205",
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
            "name": "PLUType",
            "type": "Option",
            "value": "Item",
            "System": false
          },
          {
            "id": 4,
            "name": "PLUItemNo",
            "type": "Code",
            "value": "2000-S",
            "System": false
          },
          {
            "id": 5,
            "name": "PLUVariantCode",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 6,
            "name": "PLUQuantity",
            "type": "Decimal",
            "value": 77.0,
            "System": false
          },
          {
            "id": 7,
            "name": "PLUQtyperUnitofMeasure",
            "type": "Decimal",
            "value": 1.0,
            "System": false
          },
          {
            "id": 8,
            "name": "PLUQuantity(Base)",
            "type": "Decimal",
            "value": 77.0,
            "System": false
          },
          {
            "id": 9,
            "name": "PLUUnitofMeasureCode",
            "type": "Code",
            "value": "PCS",
            "System": false
          },
          {
            "id": 10,
            "name": "PLUExpirationDate",
            "type": "Date",
            "value": null,
            "System": false
          },
          {
            "id": 11,
            "name": "PLUParentLicensePlateNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 12,
            "name": "PLUParentLicPlateLineNo",
            "type": "Integer",
            "value": null,
            "System": false
          },
          {
            "id": 13,
            "name": "PLUStatus",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 14,
            "name": "PLUSerialNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 15,
            "name": "PLULotNo",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 16,
            "name": "PLUDescription",
            "type": "Code",
            "value": "SYDNEY SWIVEL CHAIR, GREEN",
            "System": false
          },
          {
            "id": 17,
            "name": "PLUEntryQuantity",
            "type": "Code",
            "value": null,
            "System": false
          },
          {
            "id": 18,
            "name": "PLUSourceDocument",
            "type": "Option",
            "value": "Purchase Order",
            "System": false
          },
          {
            "id": 19,
            "name": "PLUSourceDocumentNo",
            "type": "Code",
            "value": "106031",
            "System": false
          },
          {
            "id": 20,
            "name": "PLUDocument",
            "type": "Option",
            "value": "Warehouse Putway",
            "System": false
          },
          {
            "id": 21,
            "name": "PLUDocumentNo",
            "type": "Code",
            "value": "10090",
            "System": false
          },
          {
            "id": 2000000000,
            "name": "$systemId",
            "type": "GUID",
            "value": "{54E5ED53-0C91-EC11-B85A-000D3A74F81B}",
            "System": false
          },
          {
            "id": 2000000001,
            "name": "SystemCreatedAt",
            "type": "DateTime",
            "value": "2022-02-18T22:44:29.197Z",
            "System": false
          },
          {
            "id": 2000000002,
            "name": "SystemCreatedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": false
          },
          {
            "id": 2000000003,
            "name": "SystemModifiedAt",
            "type": "DateTime",
            "value": "2022-02-18T22:45:23.943Z",
            "System": false
          },
          {
            "id": 2000000004,
            "name": "SystemModifiedBy",
            "type": "GUID",
            "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
            "System": false
          }
        ]
      }
    ]
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


