### API Documentation: GetWarehouseReceipt

#### Overview
The `GetWarehouseReceipt` API method retrieves detailed information about a specific Warehouse Receipt, including its associated lines and related License Plates (LPs). This method is essential for tracking warehouse receipt operations, enabling users to view all relevant details in a structured JSON format.

#### Request Structure
```json
{
  "ProcessMethod": "GetWarehouseReceipt",
  "Parameters": [
    {
      "WsheDocumentNo": "WR-000001",
      "WarehouseEmployee": "EMP001"
    }
  ]
}
```

#### Parameters
- **WsheDocumentNo**: The Warehouse Receipt document number to retrieve (e.g., `"WR-000001"`).
- **WarehouseEmployee**: The ID of the warehouse employee associated with the receipt (e.g., `"EMP001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWarehouseReceipt",
  "Parameters": [
    {
      "WsheDocumentNo": "WR-000001",
      "WarehouseEmployee": "EMP001"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehouseReceiptHeader": [
    {
      "No": "WHSE REC-00171",
      "LocationCode": "MAIN",
      "NoSeries": "WHSE REC",
      "PostingDate": "2024-08-13",
      "AssignedUserID": "",
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00171",
          "LineNo": 10000,
          "ItemNo": "D0BDBD",
          "BinCode": "MAIN",
          "VariantCode": "B60W225",
          "Quantity": 200.0,
          "QtyBase": 200.0,
          "QtyToReceive": 0.0,
          "QtyReceived": 2.0,
          "QtyOutstanding": 198.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 198.0
        },
        {
          "No": "WHSE REC-00171",
          "LineNo": 20000,
          "ItemNo": "D0BDBD",
          "BinCode": "MAIN",
          "VariantCode": "B80W245",
          "Quantity": 250.0,
          "QtyBase": 250.0,
          "QtyToReceive": 0.0,
          "QtyReceived": 0.0,
          "QtyOutstanding": 250.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 250.0
        }
      ],
      "LicensePlates": []
    }
  ],
  "Duration": "430 milliseconds"
}
```

#### Explanation
- **WarehouseReceiptHeader**: The main object containing all details about the warehouse receipt.
  - **No**: The Warehouse Receipt number (e.g., `"WR-000001"`).
  - **LocationCode**: The code of the warehouse location (e.g., `"LOC01"`).
  - **NoSeries**: The number series used for the receipt (e.g., `"WSH-001"`).
  - **PostingDate**: The date the receipt was posted (e.g., `"2024-08-15"`).
  - **AssignedUserID**: The ID of the user assigned to this receipt (e.g., `"EMP001"`).
  - **WarehouseReceiptLines**: An array containing all lines associated with the receipt.
    - **LineNo**: The line number within the receipt (e.g., `10000`).
    - **ItemNo**: The item number associated with this line (e.g., `"ITEM001"`).
    - **VariantCode**: The variant code for the item, if any (e.g., `"VAR001"`).
    - **Quantity**: The total quantity of items in this line (e.g., `10`).
    - **QtyBase**: The base quantity (e.g., `10`).
    - **QtyToReceive**: The quantity to be received (e.g., `5`).
    - **QtyReceived**: The quantity already received (e.g., `5`).
    - **QtyOutstanding**: The outstanding quantity (e.g., `5`).
    - **UnitofMeasureCode**: The unit of measure code for the item (e.g., `"PCS"`).
    - **QtyperUnitofMeasure**: The quantity per unit of measure (e.g., `1`).
    - **NewQtyOutstanding**: The new outstanding quantity (e.g., `5`).
  - **LicensePlates**: An array containing details of the license plates associated with this receipt.
    - **LPDocumentNo**: The document number of the license plate (e.g., `"LP-000001"`).
    - **LicensePlateStatus**: The status of the license plate (e.g., `"Received"`).
    - **ParentLPNo**: The parent license plate number, if any (e.g., `""`).
    - **ZoneCode**: The warehouse zone code (e.g., `"ZONE01"`).
    - **LocationCode**: The location code (e.g., `"LOC01"`).
    - **BinCode**: The bin code where the license plate is located (e.g., `"BIN001"`).
    - **WhseDocumentNo**: The warehouse document number associated with the license plate (e.g., `"WR-000001"`).
    - **SystemCreatedAt**: The date and time the license plate was created (e.g., `"2024-08-15T12:34:56Z"`).
    - **SystemCreatedBy**: The user who created the license plate (e.g., `"EMP001"`).
    - **LPTotalQuantities**: The total quantities in the license plate (e.g., `10`).
    - **LPLines**: An array containing lines associated with this license plate.
      - **LineNo**: The line number within the license plate (e.g., `10000`).
      - **ItemNo**: The item number (e.g., `"ITEM001"`).
      - **VariantCode**: The variant code (e.g., `"VAR001"`).
      - **SerialNo**: The serial number of the item, if any (e.g., `"SN001"`).
      - **LotNo**: The lot number of the item, if any (e.g., `"LOT001"`).
      - **Description**: The description of the item (e.g., `"Item Description"`).
      - **Quantity**: The quantity in this line (e.g., `10`).
      - **UnitofMeasure**: The unit of measure for the item (e.g., `"PCS"`).
    - **ChildLPs**: An array containing child license plates, if any.

#### Summary
The `GetWarehouseReceipt` method provides a comprehensive overview of a Warehouse Receipt, including its lines and associated License Plates. This API is essential for warehouse management, offering detailed insights into receipt operations, enabling effective tracking and management of inventory within the system.