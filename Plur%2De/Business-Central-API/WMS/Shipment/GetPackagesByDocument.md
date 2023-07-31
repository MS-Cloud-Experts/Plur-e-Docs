**Request:** 

```
{
  "ProcessMethod": "GetPackagesByDocument",
  "Parameters": [
    {
      "No": "WHSE PICK-00005"
    }
  ]
}
```


**Output** :
```
[
  {
    "PackageHeaders": {
      "No": 1,
      "WarehouseDocumentNo": "WHSE PICK-00005",
      "SourceNo": "S-ORD101011",
      "Weight": 0.0,
      "Width": 0.0,
      "Height": 0.0,
      "Depth": 0.0,
      "Status": false,
      "PackingDate": "0001-01-01T00:00:00.0000000",
      "Lines": [
        {
          "PackageNo": 1,
          "LineNo": 1000,
          "SourceNo": "S-ORD101011",
          "WarehouseDocumentNo": "WHSE PICK-00005",
          "WarehouseLineNo": 20000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1.0
        },
        {
          "PackageNo": 1,
          "LineNo": 2000,
          "SourceNo": "S-ORD101011",
          "WarehouseDocumentNo": "WHSE PICK-00005",
          "WarehouseLineNo": 20000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1.0
        }
      ],
      "ShipToAddress": {
        "ShipToName": "Adatum Corporation",
        "ShipToAddress": "192 Market Square",
        "ShipToAddress2": "",
        "ShipToCity": "Atlanta",
        "ShipToCountry_RegionCode": "US",
        "ShipToCounty": "GA"
      },
      "SystemCreatedAt": "2023-07-28T15:55:58.9600000Z",
      "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
    }
  }
]
```
