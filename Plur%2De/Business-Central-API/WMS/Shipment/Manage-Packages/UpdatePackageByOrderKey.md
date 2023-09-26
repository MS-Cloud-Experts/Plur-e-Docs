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
All package information is returned with the updated changes.

```
{
    "PackageHeaders": {
      "No": 1,
      "WarehouseDocumentNo": "WHSE PICK-00019",
      "CustomerUsername": "Dario Sanchez Mosquera",
      "CustomerEmail": "dario.sanchez@mscloudexperts.com",
      "WeightUnit": "Pounds",
      "DimensionsUnit": "Inches",
      "Weight": 5.0,
      "Width": 5.0,
      "Height": 2.0,
      "Depth": 8.0,
      "TotalQty": 4.0,
      "Status": true,
      "RegisteredPick": "REG PICK-00018",
      "PackageTrackingNo": "",
      "ShippingAgentCode": "",
      "ShippingAgentService": "",
      "PackingDate": "2023-09-18T22:19:54.6170000Z",
      "Lines": [
        {
          "PackageNo": 1,
          "LineNo": 1000,
          "SourceNo": "S-ORD101034",
          "SourceLineNo": 10000,
          "WarehouseDocumentNo": "WHSE PICK-00019",
          "WarehouseLineNo": 20000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 2.0
        },
        {
          "PackageNo": 1,
          "LineNo": 2000,
          "SourceNo": "S-ORD101035",
          "SourceLineNo": 10000,
          "WarehouseDocumentNo": "WHSE PICK-00019",
          "WarehouseLineNo": 40000,
          "ItemNo": "1900-S",
          "VariantCode": "",
          "QtyToHandle": 2.0
        }
      ],
      "ShipToAddress": {
        "Name": "Adatum Corporation",
        "Company": "Adventure",
        "Address1": "192 Market Square",
        "Address2": "",
        "City": "Atlanta",
        "State": "GA",
        "Country": "GA",
        "PostalCode": "31772",
        "Phone": "US"
      },
      "BillToAddress": {
        "Name": "Adatum Corporation",
        "Company": "Adventure",
        "Address1": "192 Market Square",
        "Address2": "",
        "City": "Atlanta",
        "State": "GA",
        "Country": "GA",
        "PostalCode": "31772",
        "Phone": "US"
      },
      "SystemCreatedAt": "2023-09-18T22:19:55.1900000Z",
      "SystemCreatedBy": "{2BEFFABC-4F0A-40E0-8454-4F8B442532AF}"
    }
```


