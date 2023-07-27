**Request:**
```
{
  "ProcessMethod": "CreatePackageShipmentSingle",
  "Parameters": [
    {
      "No": "WHSE PICK-00005",
      "LineNo": "20000",
      "Quantity": 1,
      "Weight": 2,
      "Width": 3,
      "Height": 4,
      "Depth": 5,
      "Status": true,
      "ShippingAgentCode": "DHL",
      "ShippingAgentServiceCode": "DHL",
      "ShippingCost": "20000",
      "PackingDate": "2023-07-27T18:00:00",
      "PackageTrackingNo": "000000077787"
    }
  ]
}
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

