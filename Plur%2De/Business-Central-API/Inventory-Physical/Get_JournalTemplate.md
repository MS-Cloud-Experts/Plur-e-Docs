**ProcessMethod**: Get_JournalTemplate

**Description**:
This method returns an array of Journal Template Type.

**Input**:
**Parameters**: 
-	**Type**: Specific Journal Template Type

    
```
    value(0; "Item") { Caption = 'Item'; }
    value(1; "Transfer") { Caption = 'Transfer'; }
    value(2; "Phys. Inventory") { Caption = 'Phys. Inventory'; }
    value(3; "Revaluation") { Caption = 'Revaluation'; }
    value(4; "Consumption") { Caption = 'Consumption'; }
    value(5; "Output") { Caption = 'Output'; }
    value(6; "Capacity") { Caption = 'Capacity'; }
    value(7; "Prod. Order") { Caption = 'Prod. Order'; }
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
  "ItemJournalTemplate": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "Description": "Phys. Inventory journal",
      "Type": "Phys. Inventory",
      "Batch": [
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "COLETTE",
          "Description": "Final Inventory ",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        },
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "DARIO",
          "Description": "",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        },
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "DEFAULT",
          "Description": "Default Journal",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        },
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "EVELINA",
          "Description": "",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        },
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "IVAN",
          "Description": "",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        },
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "JUANJ",
          "Description": "",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        },
        {
          "JournalTemplateName": "PHYS. INVE",
          "Name": "TULIO",
          "Description": "",
          "NoSeries": "",
          "ReasonCode": "",
          "PostingNoSeries": ""
        }
      ]
    }
  ],
  "Duration": "47 milliseconds"
}
```

**Errors**:
```
```


