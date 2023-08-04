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
      "WarehouseDocumentNo": "WHSE PICK-00006",
      "SourceNo": "S-ORD101015",
      "Weight": 2.0,
      "Width": 3.0,
      "Height": 4.0,
      "Depth": 5.0,
      "TotalQty": 5.0,
      "Status": true,
      "PackageTrackingNo": "000000077787",
      "ShippingAgentCode": "DHL",
      "ShippingAgentService": "DHL",
      "PackingDate": "2023-07-27T18:00:00.0000000Z",
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
        },
        {
          "PackageNo": 1,
          "LineNo": 2000,
          "SourceNo": "S-ORD101015",
          "WarehouseDocumentNo": "WHSE PICK-00006",
          "WarehouseLineNo": 40000,
          "ItemNo": "1900-S",
          "VariantCode": "",
          "QtyToHandle": 4.0
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
      "SystemCreatedAt": "2023-08-04T20:33:56.9200000Z",
      "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
    }
  }
]
```
