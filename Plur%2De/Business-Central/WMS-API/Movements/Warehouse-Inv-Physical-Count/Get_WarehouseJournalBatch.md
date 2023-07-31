**ProcessMethod**: Get_WarehouseJournalBatch

**Description**:
This method returns an array of Warehouse Journal Batches

**Input**:
**Parameters**: 
-	**JournalTemplateName**: Journal Template Name.

    
**Ouput**: 
-	**WarehouseJournalTemplate**: Array of Journal Template Type

**Example**:

Request:


```
{
  "ProcessMethod": "Get_WarehouseJournalBatch",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "UserID": "USER_840E28EEE68E4F42BA1DA9E763B7CA7B"
    }
  ]
}
```


**Outputs**:
![image.png](/.attachments/image-6275bdaa-d3a4-43d3-9ee2-7642a851dc0d.png)

```
{
  "WarehouseJournalBatch": [
    {
      "id": 7310,
      "name": "WarehouseJournalBatch",
      "company": "CRONUS USA, Inc.",
      "position": "Journal Template Name=CONST(PHYSICAL I),Name=CONST(DARIO),Location Code=CONST(WMS)",
      "recordId": "Warehouse Journal Batch: PHYSICAL I,DARIO,WMS",
      "primaryKey": {
        "fieldCount": 3,
        "fields": [
          {
            "id": 1,
            "name": "JournalTemplateName",
            "type": "Code",
            "value": "PHYSICAL I",
            "System": false
          },
          {
            "id": 2,
            "name": "Name",
            "type": "Code",
            "value": "DARIO",
            "System": false
          },
          {
            "id": 7,
            "name": "LocationCode",
            "type": "Code",
            "value": "WMS",
            "System": false
          }
        ]
      },
      "fieldCount": 16,
      "fields": [
        {
          "id": 1,
          "name": "JournalTemplateName",
          "type": "Code",
          "value": "PHYSICAL I",
          "System": false
        },
        {
          "id": 2,
          "name": "Name",
          "type": "Code",
          "value": "DARIO",
          "System": false
        },
        {
          "id": 3,
          "name": "Description",
          "type": "Text",
          "value": null,
          "System": false
        },
        {
          "id": 4,
          "name": "ReasonCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 5,
          "name": "NoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 6,
          "name": "RegisteringNoSeries",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 7,
          "name": "LocationCode",
          "type": "Code",
          "value": "WMS",
          "System": false
        },
        {
          "id": 21,
          "name": "TemplateType",
          "type": "Option",
          "value": "Physical Inventory",
          "System": false
        },
        {
          "id": 7700,
          "name": "AssignedUserID",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 71017575,
          "name": "PLUAssignedUserID",
          "type": "Code",
          "value": "USER_840E28EEE68E4F42BA1DA9E763B7CA7B",
          "System": false
        },
        {
          "id": 71017576,
          "name": "PLUAssignedUserName",
          "type": "Text",
          "value": "user_840e28eee68e4f42ba1da9e763b7ca7b",
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{F29EEBCC-458C-ED11-9989-6045BD300EA8}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2023-01-04T15:38:14.8700000Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{D6194FDA-68F1-4DEA-9340-75AF3121F16F}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2023-01-04T21:16:21.4900000Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{D6194FDA-68F1-4DEA-9340-75AF3121F16F}",
          "System": false
        }
      ]
    }
  ]
}
```

**Errors**:
```
```


