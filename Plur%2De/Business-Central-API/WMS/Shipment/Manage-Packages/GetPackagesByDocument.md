### API Documentation: GetPackagesByDocument

#### Overview
The `GetPackagesByDocument` API method retrieves detailed information about packages associated with a specified warehouse document. This includes package dimensions, shipment status, customer details, itemized line information, and shipping options, providing a comprehensive view for efficient warehouse and logistics management.

#### Request Structure
```json
{
  "ProcessMethod": "GetPackagesByDocument",
  "Parameters": [
    {
      "No": "WHSE PICK-00005"
    }
  ]
}
```

#### Parameters
- **No**: The warehouse document number for which package information is requested (e.g., `"WHSE PICK-00005"`).

#### Example Request
```json
{
  "ProcessMethod": "GetPackagesByDocument",
  "Parameters": [
    {
      "No": "WHSE PICK-00005"
    }
  ]
}
```

#### Example Response
```json
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
      }
      // Additional lines omitted for brevity
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
      }
      // Additional international options omitted for brevity
    ],
    "ShipTo": {
      "Name": "ACE PERFORMER",
      "Company": "Adventure Sports USA",
      "Address1": "16842 MC GREGOR BLVD.",
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
      "City": "Fort Myers",
      "State": "Florida",
      "Country": "US",
      "PostalCode": "33908",
      "Phone": "12394893513"
    }
  }
}
```

#### Explanation
- **PackageHeaders**: Object containing details for the package associated with the specified warehouse document.
  - **PackageNo**: The unique package identifier.
  - **SourceNo**: Reference to the source warehouse shipment.
  - **WarehouseDocumentNo**: The warehouse document number associated with the package.
  - **CustomerUsername** and **CustomerEmail**: Username and email of the customer receiving the package.
  - **WeightUnit** and **DimensionsUnit**: Units of measurement for weight and dimensions.
  - **Status**: Current status of the package (e.g., `"awaiting_shipment"`).
  - **ShippingAgentCode** and **ShippingAgentService**: Shipping agent details, including service level.
  - **PackingDate** and **ShippingDate**: Date and time the package was packed and, if available, the planned shipping date.
- **Lines**: Array of objects representing individual items in the package, including:
  - **PackageNo**: Package identifier for the item.
  - **LineNo**: Unique line number within the package.
  - **ItemNo**: Item number and other details like **VariantCode** and **SerialNo** for inventory tracking.
  - **ItemPrice** and **QtyToHandle**: Price per item and quantity in the package.
- **GenerateInternationalOptions**: Customs-related details for international shipments, including:
  - **CustomsItemId**: Identifier linking the item to customs.
  - **Description**: Description of the item for customs.
  - **CountryOfOrigin**: Country where the item was manufactured.
  - **nonDelivery**: Instructions for handling undeliverable items.
- **ShipTo** and **BillTo**: Contains recipient’s name, address, and contact information for both shipping and billing purposes.

#### Summary
The `GetPackagesByDocument` method provides detailed package information for a specified warehouse document, assisting warehouse and logistics teams in managing shipment readiness, tracking item details, and preparing for customs requirements in international shipments. This supports a seamless shipping process and enables accurate package and inventory tracking across different stages.