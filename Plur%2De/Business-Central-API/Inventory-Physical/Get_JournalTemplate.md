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


