**ProcessMethod**: Get_WarehouseJournalTemplate

**Description**:
This method returns an array of Warehouse Journals Lines special to the physical count given a Location.

**Input**:
**Parameters**: 
-	**LocationCode**: Specific Location where you want to perform the inventory count.

**Ouput**: 
-The process will be executed correctly if it returns the lines of the Warehouse Item Journal.
-	**Warehouse_Physical_Inventory_Journal**: Array of Warehouse Journals Lines.

**Example**:

Request:


```
{
  "ProcessMethod": "Get_WarehouseJournalTemplate",
  "Parameters": []
}
```


**Outputs**:


```
{
  "id": 7309,
  "name": "WarehouseJournalTemplate",
  "company": "CRONUS USA, Inc.",
  "position": "Name=CONST()",
  "recordId": "Warehouse Journal Template: \"\"",
  "primaryKey": {
    "fieldCount": 1,
    "fields": [
      {
        "id": 1,
        "name": "Name",
        "type": "Code",
        "value": null,
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
      "value": null,
      "System": false
    },
    {
      "id": 2,
      "name": "Description",
      "type": "Text",
      "value": null,
      "System": false
    },
    {
      "id": 5,
      "name": "TestReportID",
      "type": "Integer",
      "value": null,
      "System": false
    },
    {
      "id": 6,
      "name": "PageID",
      "type": "Integer",
      "value": null,
      "System": false
    },
    {
      "id": 7,
      "name": "RegisteringReportID",
      "type": "Integer",
      "value": null,
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
      "value": "Item",
      "System": false
    },
    {
      "id": 10,
      "name": "SourceCode",
      "type": "Code",
      "value": null,
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
      "value": null,
      "System": false
    },
    {
      "id": 16,
      "name": "PageCaption",
      "type": "Text",
      "value": null,
      "System": false
    },
    {
      "id": 17,
      "name": "RegisteringReportCaption",
      "type": "Text",
      "value": null,
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
      "value": "{00000000-0000-0000-0000-000000000000}",
      "System": false
    },
    {
      "id": 2000000001,
      "name": "SystemCreatedAt",
      "type": "DateTime",
      "value": null,
      "System": false
    },
    {
      "id": 2000000002,
      "name": "SystemCreatedBy",
      "type": "GUID",
      "value": "{00000000-0000-0000-0000-000000000000}",
      "System": false
    },
    {
      "id": 2000000003,
      "name": "SystemModifiedAt",
      "type": "DateTime",
      "value": null,
      "System": false
    },
    {
      "id": 2000000004,
      "name": "SystemModifiedBy",
      "type": "GUID",
      "value": "{00000000-0000-0000-0000-000000000000}",
      "System": false
    }
  ]
}
```

**Errors**:
```
```


