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
  },
  {
    "PackageHeaders": {
      "No": 2,
      "WarehouseDocumentNo": "WHSE PICK-00019",
      "CustomerUsername": "Dario Sanchez Mosquera",
      "CustomerEmail": "dario.sanchez@mscloudexperts.com",
      "WeightUnit": "Pounds",
      "DimensionsUnit": "Inches",
      "Weight": 0.0,
      "Width": 0.0,
      "Height": 0.0,
      "Depth": 0.0,
      "TotalQty": 4.0,
      "Status": false,
      "RegisteredPick": "",
      "PackageTrackingNo": "",
      "ShippingAgentCode": "",
      "ShippingAgentService": "",
      "PackingDate": "2023-09-20T19:22:59.2170000Z",
      "Lines": [
        {
          "PackageNo": 2,
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
          "PackageNo": 2,
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
      "SystemCreatedAt": "2023-09-20T19:22:59.9030000Z",
      "SystemCreatedBy": "{2BEFFABC-4F0A-40E0-8454-4F8B442532AF}"
    }
  }
]
```
