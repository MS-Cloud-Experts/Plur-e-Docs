**Request**
```
{
  "ProcessMethod": "WriteInventoryCountV2",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-13",
      "EntryType": "Negative Adjmt.",
      "DocumentNo": "SSDS",
      "ItemNo": "SERIAL2",
      "VariantCode": "",
      "Description": "",
      "LocationCode": "FTLDL-RET",
      "SalespersPurchCode": "",
      "QtyCalculated": 3,
      "QtyPhysInventory": 2,
      "Quantity": 1,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "LineNo": 20000,
      "SerialJA": [
        {
          "LineNo": 20000,
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "",
          "SerialNo": "X14"
        },
        {
          "LineNo": 20000,
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "",
          "SerialNo": "X15"
        }
      ]
    }
  ]
}

```

**Output:**

```
{
  "WriteInventoryCountV2": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-20",
      "EntryType": "Negative Adjmt.",
      "DocumentNo": "SSDS",
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
          "SerialNo": "X10"
        },
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
        }
      ],
      "CountedSerialsJA": []
    },
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "IVAN",
      "PostingDate": "2024-06-20",
      "EntryType": "Negative Adjmt.",
      "DocumentNo": "SSDS",
      "ItemNo": "SERIAL2",
      "VariantCode": "",
      "Description": "serial2",
      "LocationCode": "FTLDL-RET",
      "SalespersPurchCode": "",
      "QtyCalculated": 3.0,
      "QtyPhysInventory": 2.0,
      "Quantity": 3.0,
      "UserID": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
      "LineNo": 20000,
      "BinCode": "",
      "UnitofMeasureCode": "EA",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "UncountedSerialsJA": [
        {
          "SerialNo": "X14"
        },
        {
          "SerialNo": "X15"
        }
      ],
      "CountedSerialsJA": [
        {
          "SerialNo": "X16"
        }
      ]
    }
  ],
  "Duration": "17 seconds 102 milliseconds"
}
```

