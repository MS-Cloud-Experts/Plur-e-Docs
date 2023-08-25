**Request:**
```
{
  "ProcessMethod": "Assign_SNLOT_to_SalesLines",
  "Parameters": [
    {
      "DocumentNo": "S-ORD101058",
      "Item_Child": [
        {
          "ItemNo": "1000",
          "LineNo": 10000,
          "TrackingInfo": [
            {
              "LotNo": "",
              "SerialNo": "SN01999",
              "ExperationDate": "2023-05-24",
              "Qty": 1
            },
            {
              "LotNo": "",
              "SerialNo": "SN01998",
              "ExperationDate": "2023-05-24",
              "Qty": 1
            }
          ]
        }
      ]
    }
  ]
}
```

**Ouput:**


```
{
  "TrackingSpecificationOpen": [
    {
      "EntryNo": 2360,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01999",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2361,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01998",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2362,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01997",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2363,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01995",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2364,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01994",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2365,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01993",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2366,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01992",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    },
    {
      "EntryNo": 2367,
      "ItemNo": "1000",
      "LocationCode": "EAST",
      "SerialNo": "SN01992",
      "LotNo": "",
      "QuantityBase": -1.0,
      "QtytoHandleBase": -1.0,
      "QtytoInvoice_Base": -1.0,
      "SourceID": "S-ORD101058",
      "SourceRefNo": 10000,
      "CreationDate": "2023-08-25"
    }
  ]
}
```

