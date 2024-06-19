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
{
  "PackageHeaders": {
    "PackageNo": 1,
    "SourceNo": "WHSE SHIP-02329",
    "WarehouseDocumentNo": "WHSE PICK-02108",
    "WarehouseShipmentNo": "WHSE SHIP-02329",
    "CustomerUsername": "ACE PERFORMER",
    "CustomerEmail": "aceperformer@embarqmail.com",
    "WeightUnit": "Pounds",
    "DimensionsUnit": "Inches",
    "Status": "awaiting_shipment",
    "OrderId": 0,
    "OrderKey": "",
    "Weight": 0.0,
    "Width": 0.0,
    "Height": 0.0,
    "Depth": 0.0,
    "TotalQty": 4.0,
    "Release": true,
    "RegisteredPick": "",
    "PackageTrackingNo": "",
    "ShippingAgentCode": "fedex",
    "ShippingAgentService": "fedex_international_priority_express",
    "PackingDate": "2024-06-19T20:49:31.7430000Z",
    "ShippingDate": "0001-01-01",
    "Lines": [
      {
        "PackageNo": 1,
        "LineNo": 1000,
        "SourceNo": "SO-03000896",
        "SourceLineNo": 30000,
        "WarehouseDocumentNo": "WHSE PICK-02108",
        "WarehouseLineNo": 90000,
        "ItemNo": "D2HGFCHAKIT",
        "VariantCode": "195",
        "SerialNo": "BT04",
        "LotNo": "",
        "ItemPrice": 630.3,
        "QtyToHandle": 1
      },
      {
        "PackageNo": 1,
        "LineNo": 2000,
        "SourceNo": "SO-03000896",
        "SourceLineNo": 30000,
        "WarehouseDocumentNo": "WHSE PICK-02108",
        "WarehouseLineNo": 110000,
        "ItemNo": "D2HGFCHAKIT",
        "VariantCode": "195",
        "SerialNo": "BT03",
        "LotNo": "",
        "ItemPrice": 630.3,
        "QtyToHandle": 1
      },
      {
        "PackageNo": 1,
        "LineNo": 3000,
        "SourceNo": "SO-03000896",
        "SourceLineNo": 40000,
        "WarehouseDocumentNo": "WHSE PICK-02108",
        "WarehouseLineNo": 130000,
        "ItemNo": "D2HGFCHAKIT",
        "VariantCode": "195",
        "SerialNo": "BT02",
        "LotNo": "",
        "ItemPrice": 630.3,
        "QtyToHandle": 1
      },
      {
        "PackageNo": 1,
        "LineNo": 4000,
        "SourceNo": "SO-03000896",
        "SourceLineNo": 40000,
        "WarehouseDocumentNo": "WHSE PICK-02108",
        "WarehouseLineNo": 150000,
        "ItemNo": "D2HGFCHAKIT",
        "VariantCode": "195",
        "SerialNo": "BT01",
        "LotNo": "",
        "ItemPrice": 630.3,
        "QtyToHandle": 1
      }
    ],
    "GenerateInternationalOptions": [
      {
        "customsItems": {
          "CustomsItemId": "SO-03000896/30000",
          "Contents": "Merchandise",
          "Description": "CHARGER KIT",
          "Quantity": 1.0,
          "Value": 630.3,
          "HarmonizedTariffCode": 0,
          "CountryOfOrigin": "CN"
        },
        "nonDelivery": "return_to_sender"
      },
      {
        "customsItems": {
          "CustomsItemId": "SO-03000896/30000",
          "Contents": "Merchandise",
          "Description": "CHARGER KIT",
          "Quantity": 1.0,
          "Value": 630.3,
          "HarmonizedTariffCode": 0,
          "CountryOfOrigin": "CN"
        },
        "nonDelivery": "return_to_sender"
      },
      {
        "customsItems": {
          "CustomsItemId": "SO-03000896/40000",
          "Contents": "Merchandise",
          "Description": "CHARGER KIT",
          "Quantity": 1.0,
          "Value": 630.3,
          "HarmonizedTariffCode": 0,
          "CountryOfOrigin": "CN"
        },
        "nonDelivery": "return_to_sender"
      },
      {
        "customsItems": {
          "CustomsItemId": "SO-03000896/40000",
          "Contents": "Merchandise",
          "Description": "CHARGER KIT",
          "Quantity": 1.0,
          "Value": 630.3,
          "HarmonizedTariffCode": 0,
          "CountryOfOrigin": "CN"
        },
        "nonDelivery": "return_to_sender"
      }
    ],
    "ShipTo": {
      "Name": "ACE PERFORMER",
      "Company": "Adventure Sports USA",
      "Address1": "16842 MC GREGOR BLVD.",
      "Address2": "",
      "City": "Fort Myers",
      "State": "Florida",
      "Country": "US",
      "PostalCode": "33908",
      "Phone": "12394893513"
    },
    "BillTo": {
      "Name": "ACE PERFORMER",
      "Company": "Adventure Sports USA",
      "Address1": "16842 MC GREGOR BLVD.",
      "Address2": "",
      "City": "Fort Myers",
      "State": "Florida",
      "Country": "US",
      "PostalCode": "33908",
      "Phone": "12394893513"
    },
    "OtherOptions": {}
  }
}
```
