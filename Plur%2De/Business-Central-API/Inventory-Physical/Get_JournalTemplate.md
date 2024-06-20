**ProcessMethod**: Get_JournalTemplate

**Description**:
This method returns an array of Journal Template Type.

**Input**:
**Parameters**: 
-	**Type**: Specific Journal Template Type

    
```
     "Item" = 0;
     "Physical Inventory" = 1;
     "Reclassification" = 2;
```


**Ouput**: 
-	**WarehouseJournalTemplate**: Array of Journal Template Type

**Example**:

Request:


```
{
  "ProcessMethod": "Get_JournalTemplate",
  "Parameters": [
    {
      "Type": "2"
    }
  ]
}
```


**Outputs**:
![image.png](/.attachments/image-ae9a6ae2-bc00-45b5-a645-5f38a7a72b8f.png)

```
{
  "id": 7309,
  "name": "WarehouseJournalTemplate",
  "company": "CRONUS USA, Inc.",
  "position": "Name=CONST(PHYSICAL I)",
  "recordId": "Warehouse Journal Template: PHYSICAL I",
  "primaryKey": {
    "fieldCount": 1,
    "fields": [
      {
        "id": 1,
        "name": "Name",
        "type": "Code",
        "value": "PHYSICAL I",
        "System": false
      }
    ]
  },
  "fieldCount": 20,
  "fields": [
    {
      "id": 1,
      "name": "Name",
      "type": "Code",
      "value": "PHYSICAL I",
      "System": false
    },
    {
      "id": 2,
      "name": "Description",
      "type": "Text",
      "value": "Physical Inventory Journal",
      "System": false
    },
    {
      "id": 5,
      "name": "TestReportID",
      "type": "Integer",
      "value": 7302,
      "System": false
    },
    {
      "id": 6,
      "name": "PageID",
      "type": "Integer",
      "value": 7326,
      "System": false
    },
    {
      "id": 7,
      "name": "RegisteringReportID",
      "type": "Integer",
      "value": 7303,
      "System": false
    },
    {
      "id": 8,
      "name": "ForceRegisteringReport",
      "type": "Boolean",
      "value": false,
      "System": false
    },
    {
      "id": 9,
      "name": "Type",
      "type": "Option",
      "value": "Physical Inventory",
      "System": false
    },
    {
      "id": 10,
      "name": "SourceCode",
      "type": "Code",
      "value": "WHPHYSINVT",
      "System": false
    },
    {
      "id": 11,
      "name": "ReasonCode",
      "type": "Code",
      "value": null,
      "System": false
    },
    {
      "id": 15,
      "name": "TestReportCaption",
      "type": "Text",
      "value": "Whse. Invt.-Registering - Test",
      "System": false
    },
    {
      "id": 16,
      "name": "PageCaption",
      "type": "Text",
      "value": "Warehouse Physical Inventory Journal",
      "System": false
    },
    {
      "id": 17,
      "name": "RegisteringReportCaption",
      "type": "Text",
      "value": "Warehouse Register - Quantity",
      "System": false
    },
    {
      "id": 19,
      "name": "NoSeries",
      "type": "Code",
      "value": null,
      "System": false
    },
    {
      "id": 20,
      "name": "RegisteringNoSeries",
      "type": "Code",
      "value": null,
      "System": false
    },
    {
      "id": 30,
      "name": "IncrementBatchName",
      "type": "Boolean",
      "value": false,
      "System": false
    },
    {
      "id": 2000000000,
      "name": "$systemId",
      "type": "GUID",
      "value": "{55F8BB4B-FB85-ED11-9989-6045BD300744}",
      "System": false
    },
    {
      "id": 2000000001,
      "name": "SystemCreatedAt",
      "type": "DateTime",
      "value": "2022-12-27T15:29:48.2230000Z",
      "System": false
    },
    {
      "id": 2000000002,
      "name": "SystemCreatedBy",
      "type": "GUID",
      "value": "{764B9B04-4C01-40F0-8393-82DE7875142A}",
      "System": false
    },
    {
      "id": 2000000003,
      "name": "SystemModifiedAt",
      "type": "DateTime",
      "value": "2022-12-27T15:29:48.2230000Z",
      "System": false
    },
    {
      "id": 2000000004,
      "name": "SystemModifiedBy",
      "type": "GUID",
      "value": "{764B9B04-4C01-40F0-8393-82DE7875142A}",
      "System": false
    }
  ]
}
```

**Errors**:
```
```


