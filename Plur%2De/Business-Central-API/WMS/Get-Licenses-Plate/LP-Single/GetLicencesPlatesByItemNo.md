**ProcessMethod**: GetLicencesPlatesByItemNo

**Description**:
Method to return a list of License Plates based on the ItemNo filter.

**Input**:
Parameters: 
-	ItemNo: Represents the number of the Item to which an LP has been assigned.

**Ouput**: List of License Plates filtered by Item No.

-	**LicensePlatesHeaders**: Array of License Plates Headers.

**Example**:

**Request**:

    "jsonRequest":"{\"ProcessMethod\":\"GetLicencesPlatesByItemNo\",\"Parameters\":[{\"ItemNo\":\"2000-S\"}]}"

Outputs:


```
{
  "LicensePlatesHeaders": [
    {
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
    }
  ]
}
```


**Errors**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": "The Licences Plate List is Empty"
  }
}
```

