### API Documentation: GetWarehouseShipment

#### Overview
The `GetWarehouseShipment` API method retrieves detailed information about a specific Warehouse Shipment, including its associated lines. This method is essential for tracking warehouse shipment operations, enabling users to view all relevant details in a structured JSON format.

#### Request Structure
```json
{
  "ProcessMethod": "GetWarehouseShipment",
  "Parameters": [
    {
      "WarehouseShipmentNo": "WS00000001"
    }
  ]
}
```

#### Parameters
- **WarehouseShipmentNo**: The Warehouse Shipment document number to retrieve (e.g., `"WS00000001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWarehouseShipment",
  "Parameters": [
    {
      "WarehouseShipmentNo": "WS00000001"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehouseShipmentHeader": {
    "No": "WS00000001",
    "LocationCode": "MAIN",
    "NoSeries": "WS",
    "BinCode": "BIN001",
    "ZoneCode": "ZONE01",
    "PostingDate": "2024-09-25",
    "ShippingAgentCode": "AGENT001",
    "ShippingAgentServiceCode": "SERVICE001",
    "ShipmentMethodCode": "METHOD001",
    "ShipmentDate": "2024-09-26",
    "Status": "Shipped",
    "WarehouseShipmentLines": [
      {
        "No": "WS00000001",
        "LineNo": 10000,
        "SourceType": "Sales Order",
        "SourceSubtype": "Standard",
        "SourceNo": "SO000001",
        "SourceLineNo": 10000,
        "LocationCode": "MAIN",
        "BinCode": "BIN001",
        "ZoneCode": "ZONE01",
        "ItemNo": "ITEM001",
        "Quantity": 50,
        "QtyBase": 50,
        "QtyToShip": 10,
        "QtyShipped": 10,
        "QtyOutstanding": 40,
        "UnitofMeasureCode": "PCS",
        "QtyPerUnitofMeasure": 1,
        "VariantCode": "VAR001"
      }
    ]
  }
}
```

#### Explanation
- **WarehouseShipmentHeader**: The main object containing all details about the warehouse shipment.
  - **No**: The Warehouse Shipment document number (e.g., `"WS00000001"`).
  - **LocationCode**: The code of the warehouse location (e.g., `"MAIN"`).
  - **NoSeries**: The number series used for the shipment (e.g., `"WS"`).
  - **BinCode**: The bin code where the items are stored (e.g., `"BIN001"`).
  - **ZoneCode**: The warehouse zone code (e.g., `"ZONE01"`).
  - **PostingDate**: The date the shipment was posted (e.g., `"2024-09-25"`).
  - **ShippingAgentCode**: The code of the shipping agent (e.g., `"AGENT001"`).
  - **ShippingAgentServiceCode**: The service code of the shipping agent (e.g., `"SERVICE001"`).
  - **ShipmentMethodCode**: The code of the shipment method (e.g., `"METHOD001"`).
  - **ShipmentDate**: The date the shipment is scheduled to ship (e.g., `"2024-09-26"`).
  - **Status**: The current status of the shipment (e.g., `"Shipped"`).
  - **WarehouseShipmentLines**: An array containing all lines associated with the shipment.
    - **No**: The Warehouse Shipment document number (e.g., `"WS00000001"`).
    - **LineNo**: The line number within the shipment (e.g., `10000`).
    - **SourceType**: The source type of the shipment, such as a sales order (e.g., `"Sales Order"`).
    - **SourceSubtype**: The subtype of the source (e.g., `"Standard"`).
    - **SourceNo**: The document number of the source (e.g., `"SO000001"`).
    - **SourceLineNo**: The line number within the source document (e.g., `10000`).
    - **ItemNo**: The item number (e.g., `"ITEM001"`).
    - **Quantity**: The total quantity of the item in this line (e.g., `50`).
    - **QtyBase**: The base quantity (e.g., `50`).
    - **QtyToShip**: The quantity to be shipped (e.g., `10`).
    - **QtyShipped**: The quantity already shipped (e.g., `10`).
    - **QtyOutstanding**: The outstanding quantity (e.g., `40`).
    - **UnitofMeasureCode**: The unit of measure code for the item (e.g., `"PCS"`).
    - **QtyPerUnitofMeasure**: The quantity per unit of measure (e.g., `1`).
    - **VariantCode**: The variant code for the item, if any (e.g., `"VAR001"`).

#### Summary
The `GetWarehouseShipment` method provides a detailed overview of a Warehouse Shipment, including its header and associated lines. This API is essential for tracking shipments in the warehouse, enabling efficient management of inventory and logistics.