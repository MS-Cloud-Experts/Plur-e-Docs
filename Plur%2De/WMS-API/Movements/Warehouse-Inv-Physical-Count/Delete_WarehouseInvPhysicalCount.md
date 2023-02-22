**ProcessMethod**: Delete_WarehouseInvPhysicalCount

**Description**:
This method allows you to update the physical quantities counted in a Warehouse Inv Journal.

**Input**:
**Parameters**: 
-	**JournalTemplateName**: JournalTemplateName.
-	**JournalBatchName**: JournalBatchName.
-	**LineNo**: LineNo.
-	**LocationCode**: Specific Location where you want to perform 
-	**LPDocumentNo**: Specific LP Document No. where you want to perform the inventory count.

```
{
  "Delete_Physical_Inventory_Journal": [
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
          "name": "LocationCode",
          "value": "CCC",   
        }, 
        {
          "name": "LPDocumentNo",
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
          "value": 10000,
        },
        {
          "name": "LocationCode",
          "value": "CCC",   
        }, 
        {
          "name": "LPDocumentNo",
          "value": "LP000442",      
        }
      ]
    }
  ]
}
```

**Output**: 
-The process will be executed correctly if it returns Yes.



