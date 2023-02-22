**ProcessMethod**: Delete_WarehouseInvPhysicalCount

**Description**:
This method allows you to update the physical quantities counted in a Warehouse Inv Journal.

**Input**:
**Parameters**: 
-	**JournalTemplateName**: JournalTemplateName.
-	**JournalBatchName**: JournalBatchName.
-	**LineNo**: LineNo.
-	**LocationCode**: Specific Location where you want to perform 
-	**LPDocumentNo**: Specific LP Document No where you want to perform the inventory count.

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
}
```

**Business Central:**
![image.png](/.attachments/image-0e6b23cc-9dc3-493e-87b7-b22b326de9e4.png)

**Example**:

Request:


```
{
  "ProcessMethod": "Write_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "Warehouse_Physical_Inventory_Journal": [
        {
          "name": "WarehouseJournalLine",
          "fields": [
            {
              "name": "JournalTemplateName",
              "value": "PHYSICAL I"
            },
            {
              "name": "JournalBatchName",
              "value": "PLUR-E"
            },
            {
              "name": "LineNo",
              "value": 10000
            },
            {
              "name": "RegisteringDate",
              "value": "2022-04-19"
            },
            {
              "name": "LocationCode",
              "value": "CCC"
            },
            {
              "name": "ItemNo",
              "value": "1900-S"
            },
            {
              "name": "Qty(PhysInventory)",
              "value": 15
            },
            {
              "name": "UserID",
              "value": "IVAN.LABRADOR1"
            },
            {
              "name": "VariantCode",
              "value": null
            },
            {
              "name": "SerialNo",
              "value": null
            },
            {
              "name": "LotNo",
              "value": null
            },
            {
              "name": "PLULicensePlates",
              "value": "LP000442"
            }
          ]
        },
        {
          "name": "WarehouseJournalLine",
          "fields": [
            {
              "name": "JournalTemplateName",
              "value": "PHYSICAL I"
            },
            {
              "name": "JournalBatchName",
              "value": "PLUR-E"
            },
            {
              "name": "LineNo",
              "value": 20000
            },
            {
              "name": "RegisteringDate",
              "value": "2022-04-19"
            },
            {
              "name": "LocationCode",
              "value": "CCC"
            },
            {
              "name": "ItemNo",
              "value": "1900-S"
            },
            {
              "name": "Qty(PhysInventory)",
              "value": 5
            },
            {
              "name": "UserID",
              "value": "IVAN.LABRADOR1"
            },
            {
              "name": "VariantCode",
              "value": null
            },
            {
              "name": "SerialNo",
              "value": null
            },
            {
              "name": "LotNo",
              "value": null
            },
            {
              "name": "PLULicensePlates",
              "value": "LP000443"
            }
          ]
        }
      ]
    }
  ]
}
```


**Output**: 
-The process will be executed correctly if it returns Yes.



