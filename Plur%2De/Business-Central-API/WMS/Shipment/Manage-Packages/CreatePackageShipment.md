### API Documentation: CreatePackageShipment

#### Overview
The `CreatePackageShipment` API method initiates a shipment for a specified warehouse pick document. This method includes the option to define packaging details, shipping options, and associated line items to be included in the shipment. The generated output provides comprehensive information about the package, including tracking details, customer information, and international shipping options, ensuring clear documentation for inventory and logistics management.

#### Request Structure
```json
{
  "ProcessMethod": "CreatePackageShipment",
  "Parameters": [
    {
      "No": "WHSE PICK-02944",
      "Weight": 0,
      "Width": 0,
      "Height": 0,
      "Depth": 0,
      "Release": true,
      "OrderId": 0,
      "OrderKey": "",
      "ShipmentStatus": 1,
      "DimensionsUnit": 0,
      "WeightUnit": 0,
      "ShippingAgentCode": "PICK AT WAREHOUSE",
      "ShippingAgentServiceCode": "Pick up",
      "ShippingCost": 0,
      "PackingDate": "2024-08-01T12:14:03.460Z",
      "PackageTrackingNo": "",
      "PackageLinesArray": [
        {
          "WarehouseDocumentNo": "WHSE PICK-02944",
          "WarehouseLineNo": 10000,
          "SourceNo": "SOB2B-101995",
          "ItemNo": "K3FKWPX2V",
          "VariantCode": "093180",
          "QtyToHandle": 1,
          "SourceLineNo": 10000,
          "SerialNo": "K3FKWPX2V093180027",
          "LotNo": ""
        },
        {
          "WarehouseDocumentNo": "WHSE PICK-02944",
          "WarehouseLineNo": 30000,
          "SourceNo": "SOB2B-101995",
          "ItemNo": "K4FWVSWNG200XXX",
          "VariantCode": "",
          "QtyToHandle": 1,
          "SourceLineNo": 20000,
          "SerialNo": "K4FWVSWNG200011",
          "LotNo": ""
        }
      ],
      "WarehouseEmployee": "MARCELLUS.SMITH"
    }
  ]
}
```

**ShipmentStatus:** 
  - value(0; Awaiting_payment)
  - value(1; Awaiting_shipment)
  - value(2; Pending_fulfillmentm)
  - value(3; On_hold)

**DimensionsUnit:**
  - value(0; Inches)
  - value(1; Centimeters)

**WeightUnit:**
   - value(0; Pounds)
   - value(1; Ounces)
   - value(2; Grams)


#### Parameters
- **No**: The document number for the warehouse pick associated with the shipment (e.g., `"WHSE PICK-02944"`).
- **Weight**: Total weight of the package.
- **Width**, **Height**, **Depth**: Dimensions of the package.
- **Release**: Boolean indicating if the package is released for shipment.
- **OrderId** and **OrderKey**: Optional fields for tracking associated orders.
- **ShipmentStatus**: Status indicator for the shipment.
- **DimensionsUnit** and **WeightUnit**: Units used for dimensions and weight (e.g., inches and pounds).
- **ShippingAgentCode**: Code for the selected shipping agent (e.g., `"PICK AT WAREHOUSE"`).
- **ShippingAgentServiceCode**: Code for the specific service provided by the shipping agent.
- **ShippingCost**: Cost of shipping.
- **PackingDate**: Date and time the package was packed.
- **PackageTrackingNo**: Tracking number for the package.
- **PackageLinesArray**: Array of line items included in the shipment. Each line contains:
  - **WarehouseDocumentNo**: Document number associated with the line item.
  - **WarehouseLineNo**: Line number within the warehouse document.
  - **SourceNo**: Source document number (e.g., sales order).
  - **ItemNo**: Item number in the shipment.
  - **VariantCode**: Optional code for variant of the item.
  - **QtyToHandle**: Quantity to be handled for this line.
  - **SerialNo** and **LotNo**: Serial and lot numbers for the item, if applicable.

#### Example Request
```json
{
  "ProcessMethod": "CreatePackageShipment",
  "Parameters": [
    {
      "No": "WHSE PICK-02944",
      "Weight": 0,
      "Width": 0,
      "Height": 0,
      "Depth": 0,
      "Release": true,
      "OrderId": 0,
      "OrderKey": "",
      "ShipmentStatus": 1,
      "DimensionsUnit": 0,
      "WeightUnit": 0,
      "ShippingAgentCode": "PICK AT WAREHOUSE",
      "ShippingAgentServiceCode": "Pick up",
      "ShippingCost": 0,
      "PackingDate": "2024-08-01T12:14:03.460Z",
      "PackageTrackingNo": "",
      "PackageLinesArray": [
        {
          "WarehouseDocumentNo": "WHSE PICK-02944",
          "WarehouseLineNo": 10000,
          "SourceNo": "SOB2B-101995",
          "ItemNo": "K3FKWPX2V",
          "VariantCode": "093180",
          "QtyToHandle": 1,
          "SourceLineNo": 10000,
          "SerialNo": "K3FKWPX2V093180027",
          "LotNo": ""
        },
        {
          "WarehouseDocumentNo": "WHSE PICK-02944",
          "WarehouseLineNo": 30000,
          "SourceNo": "SOB2B-101995",
          "ItemNo": "K4FWVSWNG200XXX",
          "VariantCode": "",
          "QtyToHandle": 1,
          "SourceLineNo": 20000,
          "SerialNo": "K4FWVSWNG200011",
          "LotNo": ""
        }
      ],
      "WarehouseEmployee": "MARCELLUS.SMITH"
    }
  ]
}
```

#### Example Response
```json
{
  "PackageNo": 1,
  "SourceNo": "WHSE SHIP-04484",
  "WarehouseDocumentNo": "WHSE PICK-04065",
  "WarehouseShipmentNo": "WHSE SHIP-04484",
  "CustomerUsername": "Francisco Javier Diéguez Álvarez",
  "CustomerEmail": "",
  "WeightUnit": "Pounds",
  "DimensionsUnit": "Inches",
  "Status": "shipped",
  "OrderId": 0,
  "OrderKey": "",
  "Weight": 0.0,
  "Width": 0.0,
  "Height": 0.0,
  "Depth": 0.0,
  "TotalQty": 2.0,
  "Release": true,
  "RegisteredPick": "",
  "PackageTrackingNo": "",
  "ShippingAgentCode": "pick at warehouse",
  "ShippingAgentService": "",
  "PackingDate": "2024-08-01T12:14:03.4600000Z",
  "ShippingDate": "0001-01-01",
  "Lines": [
    {
      "PackageNo": 1,
      "LineNo": 1000,
      "SourceNo": "SOB2B-101995",
      "SourceLineNo": 10000,
      "WarehouseDocumentNo": "WHSE PICK-04065",
      "WarehouseLineNo": 10000,
      "ItemNo": "K3FKWPX2V",
      "VariantCode": "093180",
      "SerialNo": "K3FKWPX2V093180027",
      "LotNo": "",
      "ItemPrice": 483.0,
      "QtyToHandle": 1
    },
    {
      "PackageNo": 1,
      "LineNo": 2000,
      "SourceNo": "SOB2B-101995",
      "SourceLineNo": 20000,
      "WarehouseDocumentNo": "WHSE PICK-04065",
      "WarehouseLineNo": 30000,
      "ItemNo": "K4FWVSWNG200XXX",
      "VariantCode": "",
      "SerialNo": "K4FWVSWNG200011",
      "LotNo": "",
      "ItemPrice": 107.0,
      "QtyToHandle": 1
    }
  ],
  "GenerateInternationalOptions": {
    "Contents": "merchandise",
    "customsItems": [
      {
        "CustomsItemId": "SOB2B-101995/10000",
        "Description": "FOIL KIT WING PACK MKII FUSE MED",
        "Quantity": 1,
        "Value": 483.0,
        "HarmonizedTariffCode": "",
        "CountryOfOrigin": "CN"
      },
      {
        "CustomsItemId": "SOB2B-101995/20000",
        "Description": "V-SERIES STAB 200",
        "Quantity": 1,
        "Value": 107.0,
        "HarmonizedTariffCode": "",
        "CountryOfOrigin": "CN"
      }
    ],
    "nonDelivery": "return_to_sender"
  },
  "ShipTo": {
    "Name": "PICK UP DAVE/TODD FUERTEVENTURA",
    "Company": "Adventure Sports USA",
    "Country": "ES"
  },
  "BillTo": {
    "Name": "Francisco Javier Diéguez Álvarez",
    "Company": "Adventure Sports USA",
    "Address1": "78792423N",
    "Address2": "LUGAR MINARZO182, 15292

",
    "City": "LIRA CARNOTA A CORUNA",
    "Country": "ES"
  },
  "OtherOptions": {},
  "Duration": "2 seconds 619 milliseconds"
}
```

#### Explanation
- **PackageNo**: Unique number for the package.
- **SourceNo**, **WarehouseDocumentNo**, **WarehouseShipmentNo**: Identifiers for the source document, warehouse pick, and shipment document.
- **CustomerUsername** and **CustomerEmail**: Customer details.
- **WeightUnit** and **DimensionsUnit**: Units used (e.g., "Pounds" and "Inches").
- **Lines**: Detailed items in the package, each with:
  - **PackageNo**: Package identifier.
  - **LineNo**: Line number.
  - **ItemNo**, **VariantCode**, **SerialNo**, **LotNo**: Product details.
  - **ItemPrice**: Price per item.
  - **QtyToHandle**: Quantity handled per line.
- **GenerateInternationalOptions**: Customs information.
- **ShipTo** and **BillTo**: Shipping and billing details.
  
#### Summary
The `CreatePackageShipment` method streamlines creating and tracking packages with specific line items, providing full documentation for each shipped item, customs compliance, and customer details for complete visibility in order fulfillment.

