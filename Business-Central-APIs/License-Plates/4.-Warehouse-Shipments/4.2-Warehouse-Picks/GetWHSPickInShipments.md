### API Documentation: GetWHSPickInShipments

#### Overview
The `GetWHSPickInShipments` API method retrieves detailed information about warehouse picks associated with a specific Warehouse Shipment. This method is essential for tracking warehouse picking operations related to shipments, providing users with a structured JSON response that includes both pick headers and lines.

#### Request Structure
```json
{
  "ProcessMethod": "GetWHSPickInShipments",
  "Parameters": [
    {
      "WhseDocumentNo": "WS00000001"
    }
  ]
}
```

#### Parameters
- **WhseDocumentNo**: The Warehouse Shipment document number to retrieve picks for (e.g., `"WS00000001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWHSPickInShipments",
  "Parameters": [
    {
      "WhseDocumentNo": "WS00000001"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehousePickHeader": [
    {
      "No": "WSPICK00001",
      "LocationCode": "MAIN",
      "NoSeries": "WS-PICK",
      "AssignedUserID": "USER001",
      "AssignmentDate": "2024-09-26",
      "CompletedByPlure": false,
      "WarehousePickLines": [
        {
          "ActionType": "Pick",
          "No": "WSPICK00001",
          "WhseDocumentNo": "WS00000001",
          "LineNo": 10000,
          "ItemNo": "ITEM001",
          "VariantCode": "VAR001",
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "Description": "Item Description",
          "SourceType": "Sales Order",
          "SourceSubtype": "Standard",
          "SourceNo": "SO000001",
          "SourceLineNo": 10000,
          "LocationCode": "MAIN",
          "BinCode": "BIN001",
          "BinCodeList": ["BIN001", "BIN002"],
          "ZoneCode": "ZONE01",
          "Quantity": 50,
          "QtyToHandle": 10,
          "QtyHandled": 10,
          "QtyBase": 50,
          "QtyOutstanding": 40,
          "QtyOutstandingBase": 40,
          "UnitofMeasureCode": "PCS",
          "QtyPerUnitofMeasure": 1
        }
      ]
    }
  ],
  "WarehousePicksNoCreated": [
    {
      "ItemNo": "ITEM002",
      "Quantity": 20
    }
  ]
}
```

#### Explanation
- **WarehousePickHeader**: The main object containing all details about the warehouse picks.
  - **No**: The pick document number (e.g., `"WSPICK00001"`).
  - **LocationCode**: The warehouse location code (e.g., `"MAIN"`).
  - **NoSeries**: The series used for the pick document (e.g., `"WS-PICK"`).
  - **AssignedUserID**: The user ID assigned to this pick (e.g., `"USER001"`).
  - **AssignmentDate**: The date the pick was assigned (e.g., `"2024-09-26"`).
  - **CompletedByPlure**: Indicates if the pick was completed by the Plure system (e.g., `false`).
  - **WarehousePickLines**: An array of lines associated with the pick document.
    - **ActionType**: The type of action performed (e.g., `"Pick"`).
    - **No**: The pick document number (e.g., `"WSPICK00001"`).
    - **WhseDocumentNo**: The Warehouse Shipment document number (e.g., `"WS00000001"`).
    - **LineNo**: The line number within the pick document (e.g., `10000`).
    - **ItemNo**: The item number (e.g., `"ITEM001"`).
    - **VariantCode**: The variant code for the item (e.g., `"VAR001"`).
    - **SerialNo**: The serial number of the item (e.g., `"SN001"`).
    - **LotNo**: The lot number of the item (e.g., `"LOT001"`).
    - **Description**: The item description (e.g., `"Item Description"`).
    - **SourceType**: The source type of the pick (e.g., `"Sales Order"`).
    - **SourceSubtype**: The subtype of the source (e.g., `"Standard"`).
    - **SourceNo**: The source document number (e.g., `"SO000001"`).
    - **SourceLineNo**: The source line number (e.g., `10000`).
    - **LocationCode**: The location code (e.g., `"MAIN"`).
    - **BinCode**: The bin code where the item is stored (e.g., `"BIN001"`).
    - **BinCodeList**: The list of bins used for this line (e.g., `["BIN001", "BIN002"]`).
    - **ZoneCode**: The warehouse zone code (e.g., `"ZONE01"`).
    - **Quantity**: The total quantity of the item in this line (e.g., `50`).
    - **QtyToHandle**: The quantity to be handled (e.g., `10`).
    - **QtyHandled**: The quantity already handled (e.g., `10`).
    - **QtyBase**: The base quantity (e.g., `50`).
    - **QtyOutstanding**: The outstanding quantity (e.g., `40`).
    - **QtyOutstandingBase**: The outstanding base quantity (e.g., `40`).
    - **UnitofMeasureCode**: The unit of measure code (e.g., `"PCS"`).
    - **QtyPerUnitofMeasure**: The quantity per unit of measure (e.g., `1`).

- **WarehousePicksNoCreated**: An array listing items and their quantities where no picks have been created.
  - **ItemNo**: The item number (e.g., `"ITEM002"`).
  - **Quantity**: The quantity outstanding (e.g., `20`).

#### Summary
The `GetWHSPickInShipments` method provides detailed insights into Warehouse Pick operations for a specific Warehouse Shipment. This API offers a comprehensive view of both pick headers and lines, along with any discrepancies in pick creation, enabling better inventory management and tracking in warehouse operations.