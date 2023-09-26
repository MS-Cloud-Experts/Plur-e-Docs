**ShippingAgentCode**
An API must be created that returns the previous Agents created since it must be as is.

![image.png](/.attachments/image-a0ab3912-630e-4e3e-81cc-37ac1d799c0a.png)

**ShipmentStatus:**

value(0; Awaiting_payment)
value(1; Awaiting_shipment)
value(2; Pending_fulfillmentm)
value(3; On_hold)

**Request:**
```
{
  "ProcessMethod": "UpdatePackageByOrderKey",
  "Parameters": [
    {
      "OrderKey": 123456789123456,
      "ShipmentStatus" : 1,
      "ShippingAgentCode": "DHL",
      "ShippingDate": "2023-07-27T18:00:00",
      "PackageTrackingNo": "000000077787",
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


