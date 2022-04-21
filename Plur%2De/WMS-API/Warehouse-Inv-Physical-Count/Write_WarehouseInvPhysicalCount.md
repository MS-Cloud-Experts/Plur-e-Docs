**ProcessMethod**: Write_WarehouseInvPhysicalCount

**Description**:
This method allows you to update the physical quantities counted in a Warehouse Inv Journal.

**Input**:
**Parameters**: 
-	**JournalTemplateName**: Specific Location where you want to perform the inventory count.
-	**JournalBatchName**: Specific Location where you want to perform the inventory count.
-	**LineNo**: Specific Location where you want to perform the inventory count.
-	**RegisteringDate**: Specific Location where you want to perform the inventory count.
-	**LocationCode**: Specific Location where you want to perform the inventory count.
-	**ItemNo**: Specific Location where you want to perform the inventory count.
-	**Qty(PhysInventory)**: Specific Location where you want to perform the inventory count.
-	**UserID**: Specific Location where you want to perform the inventory count.
-	**VariantCode**: Specific Location where you want to perform the inventory count.
-	**SerialNo**: Specific Location where you want to perform the inventory count.
-	**SerialNo**: Specific Location where you want to perform the inventory count.
-	**PLULicensePlates**: Specific Location where you want to perform the inventory count.

```
{
  "Warehouse_Physical_Inventory_Journal": [
    {
      "name": "WarehouseJournalLine",
      "fields": [
        {
          "name": "JournalTemplateName",
          "value": "PHYSICAL I",
        },
        {
          "name": "JournalBatchName",
          "value": "PLUR-E",
        },
        {
          "name": "LineNo",
          "value": 10000,
        },
        {
          "name": "RegisteringDate",
          "value": "2022-04-19",
        },
        {
          "name": "LocationCode",
          "value": "CCC",   
        },
        {
          "name": "ItemNo",
          "value": "1900-S",
        },
        {
          "name": "Qty(PhysInventory)",
          "value": null,
        },
        {
          "name": "UserID",
          "value": "IVAN.LABRADOR1",    
        },
        {
          "name": "VariantCode",
          "value": null,
        },
        {
          "name": "SerialNo",
          "value": null,      
        },
        {
          "name": "LotNo",
          "value": null,     
        },   
        {
          "name": "PLULicensePlates",
          "value": "LP000442",      
        }
      ]
    },
    {
      "name": "WarehouseJournalLine",
      "fields": [
        {
          "name": "JournalTemplateName",
          "value": "PHYSICAL I",       
        },
        {
          "name": "JournalBatchName",
          "value": "PLUR-E",      
        },
        {
          "name": "LineNo",
          "value": 20000,
        },
        {
          "name": "RegisteringDate",
          "value": "2022-04-19",
        },
        {
          "name": "LocationCode",
          "value": "CCC",
        },
        {
          "name": "ItemNo",
          "value": "1900-S",       
        },
        {
          "name": "Qty(PhysInventory)",
          "value": null,      
        },
        {
          "name": "UserID",
          "value": "IVAN.LABRADOR1",
        },
        {
          "name": "VariantCode",
          "value": null,
        },
        {
          "name": "SerialNo",
          "value": null,
        },
        {
          "name": "LotNo",
          "value": null,
        },
        {
          "name": "PLULicensePlates",
          "value": "LP000443",    
        }
      ]
    }
  ]
}
}
```

**Example**:

Request:

`    "jsonRequest":"{\"ProcessMethod\":\"Write_WarehouseInvPhysicalCount\",\"Parameters\":[{\"Warehouse_Physical_Inventory_Journal\": [{\"name\": \"WarehouseJournalLine\",\"fields\": [{\"name\": \"JournalTemplateName\",\"value\": \"PHYSICAL I\",},{\"name\": \"JournalBatchName\",\"value\": \"PLUR-E\",},{\"name\": \"LineNo\",\"value\": 10000,},{\"name\": \"RegisteringDate\",\"value\": \"2022-04-19\",},{\"name\": \"LocationCode\",\"value\": \"CCC\", },{\"name\": \"ItemNo\",\"value\": \"1900-S\",},{\"name\": \"Qty(PhysInventory)\",\"value\": 15,},{\"name\": \"UserID\",\"value\": \"IVAN.LABRADOR1\",},{\"name\": \"VariantCode\",\"value\": null,},{\"name\": \"SerialNo\",\"value\": null,},{\"name\": \"LotNo\",\"value\": null, }, {\"name\": \"PLULicensePlates\",\"value\": \"LP000442\",}]},{\"name\": \"WarehouseJournalLine\",\"fields\": [{\"name\": \"JournalTemplateName\",\"value\": \"PHYSICAL I\", },{\"name\": \"JournalBatchName\",\"value\": \"PLUR-E\",},{\"name\": \"LineNo\",\"value\": 20000,},{\"name\": \"RegisteringDate\",\"value\": \"2022-04-19\",},{\"name\": \"LocationCode\",\"value\": \"CCC\",},{\"name\": \"ItemNo\",\"value\": \"1900-S\", },{\"name\": \"Qty(PhysInventory)\",\"value\": 5,},{\"name\": \"UserID\",\"value\": \"IVAN.LABRADOR1\",},{\"name\": \"VariantCode\",\"value\": null,},{\"name\": \"SerialNo\",\"value\": null,},{\"name\": \"LotNo\",\"value\": null,},{\"name\": \"PLULicensePlates\",\"value\": \"LP000443\",}]}]}]}"`

**Output**: 
-The process will be executed correctly if it returns the lines of the Warehouse Item Journal.
-	**Warehouse_Physical_Inventory_Journal**: Array of Warehouse Journals Lines.


