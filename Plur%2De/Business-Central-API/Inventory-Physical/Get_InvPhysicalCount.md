**Request:**

```
{
  "ProcessMethod": "Get_InvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT"
    }
  ]
}
```

**Output:**

```
{
  "PhysicalInventoryCount": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-20",
      "EntryType": "Negative Adjmt.",
      "DocumentNo": "SOB2B-101485",
      "ItemNo": "SERIAL",
      "VariantCode": "",
      "Description": "serial",
      "LocationCode": "FTLDL-RET",
      "SalespersPurchCode": "",
      "QtyCalculated": 12.0,
      "QtyPhysInventory": 0.0,
      "Quantity": 12.0,
      "UserID": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
      "LineNo": 10000,
      "BinCode": "",
      "UnitofMeasureCode": "EA",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "UncountedSerialsJA": [
        {
          "SerialNo": "X11"
        },
        {
          "SerialNo": "X12"
        },
        {
          "SerialNo": "X13"
        },
        {
          "SerialNo": "X2"
        },
        {
          "SerialNo": "X3"
        },
        {
          "SerialNo": "X4"
        },
        {
          "SerialNo": "X5"
        },
        {
          "SerialNo": "X6"
        },
        {
          "SerialNo": "X7"
        },
        {
          "SerialNo": "X8"
        },
        {
          "SerialNo": "X9"
        },
        {
          "SerialNo": "X10"
        }
      ],
      "CountedSerialsJA": []
    },
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-20",
      "EntryType": "Negative Adjmt.",
      "DocumentNo": "SOB2B-101485",
      "ItemNo": "SERIAL2",
      "VariantCode": "",
      "Description": "serial2",
      "LocationCode": "FTLDL-RET",
      "SalespersPurchCode": "",
      "QtyCalculated": 3.0,
      "QtyPhysInventory": 2.0,
      "Quantity": 1.0,
      "UserID": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
      "LineNo": 20000,
      "BinCode": "",
      "UnitofMeasureCode": "EA",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "UncountedSerialsJA": [
        {
          "SerialNo": "X16"
        }
      ],
      "CountedSerialsJA": [
        {
          "SerialNo": "X14"
        },
        {
          "SerialNo": "X15"
        }
      ]
    }
  ],
  "Duration": "3 seconds 636 milliseconds"
}
```

![image.png](/.attachments/image-09a0bafd-2fd2-4b46-92de-fddfae1cd4ff.png)
