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
    "PackageNo": 1,
    "SourceNo": "WHSE PICK-00097",
    "WarehouseDocumentNo": "WHSE PICK-00097",
    "WarehouseShipmentNo": "WHSE SHIP-00090",
    "CustomerUsername": "Adatum Corporation",
    "CustomerEmail": "ivan.labrador@mscloudexperts.com",
    "WeightUnit": "Pounds",
    "DimensionsUnit": "Inches",
    "Status": "awaiting_shipment",
    "OrderId": 50790117,
    "OrderKey": "77bbcd49e6454c32bb6282dd9923c3e8",
    "Weight": 0.0,
    "Width": 0.0,
    "Height": 0.0,
    "Depth": 0.0,
    "TotalQty": 1.0,
    "Release": true,
    "RegisteredPick": "",
    "PackageTrackingNo": "",
    "ShippingAgentCode": "fedex",
    "ShippingAgentService": "fedex_international_priority_express",
    "PackingDate": "2024-02-20T14:57:02.6430000Z",
    "ShippingDate": "0001-01-01",
    "Lines": [
      {
        "PackageNo": 1,
        "LineNo": 1000,
        "SourceNo": "S-ORD101126",
        "SourceLineNo": 10000,
        "WarehouseDocumentNo": "WHSE PICK-00097",
        "WarehouseLineNo": 10000,
        "ItemNo": "1006",
        "VariantCode": "",
        "SerialNo": "SN00103",
        "LotNo": "",
        "ItemPrice": 777.0,
        "QtyToHandle": 1
      }
    ],
    "ShipTo": {
      "Name": "Adatum Corporation",
      "Company": "Adventure",
      "Address1": "2 Lewes Road",
      "Address2": "",
      "City": "Atlanta",
      "State": "GA",
      "Country": "US",
      "PostalCode": "31772",
      "Phone": ""
    },
    "BillTo": {
      "Name": "Adatum Corporation",
      "Company": "Adventure",
      "Address1": "192 Market Square",
      "Address2": "",
      "City": "Atlanta",
      "State": "GA",
      "Country": "US",
      "PostalCode": "31772",
      "Phone": ""
    }
  }
]
```
