**Request:**
```
[
  {
    "PackageHeaders": {
      "No": 1,
      "WarehouseDocumentNo": "WHSE PICK-00006",
      "SourceNo": "S-ORD101015",
      "Weight": 2.0,
      "Width": 3.0,
      "Height": 2.0,
      "Depth": 2.0,
      "Status": false,
      "PackingDate": "2023-07-28T20:21:20.6130000Z",
      "Lines": [
        {
          "PackageNo": 1,
          "LineNo": 1000,
          "SourceNo": "S-ORD101015",
          "WarehouseDocumentNo": "WHSE PICK-00006",
          "WarehouseLineNo": 20000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1.0
        }
      ],
      "ShipToAddress": {
        "ShipToName": "School of Fine Art",
        "ShipToAddress": "10 High Tower Green",
        "ShipToAddress2": "",
        "ShipToCity": "Miami",
        "ShipToCountry_RegionCode": "US",
        "ShipToCounty": "FL"
      },
      "SystemCreatedAt": "2023-07-28T20:18:39.2300000Z",
      "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
    }
  },
  {
    "PackageHeaders": {
      "No": 2,
      "WarehouseDocumentNo": "WHSE PICK-00006",
      "SourceNo": "S-ORD101015",
      "Weight": 0.0,
      "Width": 0.0,
      "Height": 0.0,
      "Depth": 0.0,
      "Status": false,
      "PackingDate": "0001-01-01T00:00:00.0000000",
      "Lines": [],
      "ShipToAddress": {
        "ShipToName": "School of Fine Art",
        "ShipToAddress": "10 High Tower Green",
        "ShipToAddress2": "",
        "ShipToCity": "Miami",
        "ShipToCountry_RegionCode": "US",
        "ShipToCounty": "FL"
      },
      "SystemCreatedAt": "2023-07-28T20:21:32.7770000Z",
      "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
    }
  }
]
```

**OutPut:**

```
{
  "No": 10,
  "ItemNo": "1896-S",
  "Quantity": 1.0,
  "WarehouseDocumentNo": "WHSE PICK-00005",
  "SourceNo": "S-ORD101011",
  "ShipToAddress": {
    "ShipToName": "Adatum Corporation",
    "ShipToAddress": "192 Market Square",
    "ShipToAddress2": "",
    "ShipToCity": "Atlanta",
    "ShipToCountry_RegionCode": "US",
    "ShipToCounty": "GA"
  },
  "Weight": 2.0,
  "Width": 3.0,
  "Height": 4.0,
  "Depth": 5.0,
  "Status": true,
  "PackingDate": "2023-07-27T18:00:00.0000000Z",
  "SystemCreatedAt": "2023-07-27T22:21:20.9000000Z",
  "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
}
```

**Errors:**

If you try to allocate more than what the line has available, it gives this error:

```
{
    "error": {
        "code": "Application_DialogException",
        "message": "There is no quantity to handle  CorrelationId:  006e8be7-6ae9-4bbc-acaf-d636d2155278."
    }
}
```


