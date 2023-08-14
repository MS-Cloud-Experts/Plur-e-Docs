**Request:**
```
{
  "ProcessMethod": "CreatePackageShipment",
  "Parameters": [
    {
      "No": "WHSE PICK-00006",
      "Weight": 2,
      "Width": 3,
      "Height": 4,
      "Depth": 5,
      "Status": true,
      "ShippingAgentCode": "DHL",
      "ShippingAgentServiceCode": "DHL",
      "ShippingCost": "20000",
      "PackingDate": "2023-07-27T18:00:00",
      "PackageTrackingNo": "000000077787",
      "PackageLinesArray": [
        {
          "WhsDocumentNo": "WHSE PICK-00006",
          "WhsDocumentLineNo": 20000,
          "SourceNo": "S-ORD101015",
          "ItemCode": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1
        },
        {
          "WhsDocumentNo": "WHSE PICK-00006",
          "WhsDocumentLineNo": 40000,
          "SourceNo": "S-ORD101015",
          "ItemCode": "1900-S",
          "VariantCode": "",
          "QtyToHandle": 4
        }
      ]
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

**Business Central:**
![image.png](/.attachments/image-167e2f2e-8612-43f5-8bc9-38eb136aaeca.png)

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

