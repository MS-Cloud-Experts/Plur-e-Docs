### API Documentation: GetWarehousePutAway

#### Overview
The `GetWarehousePutAway` API method retrieves detailed information about a specific Warehouse Put-Away, including its associated lines and related License Plates (LPs). This method is essential for tracking warehouse put-away operations, providing users with a structured JSON response that includes all relevant details.

#### Request Structure
```json
{
  "ProcessMethod": "GetWarehousePutAway",
  "Parameters": [
    {
      "WsheDocumentNo": "PA-000001",
      "WarehouseEmployee": "EMP002"
    }
  ]
}
```

#### Parameters
- **WsheDocumentNo**: The Warehouse Put-Away document number to retrieve (e.g., `"PA-000001"`).
- **WarehouseEmployee**: The ID of the warehouse employee associated with the put-away (e.g., `"EMP002"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWarehousePutAway",
  "Parameters": [
    {
      "WsheDocumentNo": "PA-000001",
      "WarehouseEmployee": "EMP002"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehousePutAwayHeader": [
    {
      "No": "PA-000001",
      "LocationCode": "LOC02",
      "NoSeries": "WPA-001",
      "PostingDate": "2024-08-16",
      "AssignedUserID": "EMP002",
      "WarehousePutAwayLines": [
        {
          "No": "PA-000001",
          "LineNo": 20000,
          "ItemNo": "ITEM002",
          "VariantCode": "VAR002",
          "Quantity": 20,
          "QtyBase": 20,
          "QtyToPutAway": 10,
          "QtyPutAway": 10,
          "QtyOutstanding": 10,
          "UnitofMeasureCode": "PCS",
          "QtyperUnitofMeasure": 1,
          "NewQtyOutstanding": 10
        }
      ],
      "LicensePlates": [
        {
          "LPDocumentNo": "LP-000002",
          "LicensePlateStatus": "Labeled",
          "ParentLPNo": "",
          "ZoneCode": "ZONE02",
          "LocationCode": "LOC02",
          "BinCode": "BIN002",
          "WhseDocumentNo": "PA-000001",
          "SystemCreatedAt": "2024-08-16T14:22:33Z",
          "SystemCreatedBy": "EMP002",
          "LPTotalQuantities": 20,
          "LPLines": [
            {
              "LineNo": 20000,
              "ItemNo": "ITEM002",
              "VariantCode": "VAR002",
              "SerialNo": "SN002",
              "LotNo": "LOT002",
              "Description": "Item Description",
              "Quantity": 20,
              "UnitofMeasure": "PCS"
            }
          ],
          "ChildLPs": []
        }
      ]
    }
  ]
}
```

#### Explanation
- **WarehousePutAwayHeader**: The main object containing all details about the warehouse put-away.
  - **No**: The Warehouse Put-Away number (e.g., `"PA-000001"`).
  - **LocationCode**: The code of the warehouse location (e.g., `"LOC02"`).
  - **NoSeries**: The number series used for the put-away (e.g., `"WPA-001"`).
  - **PostingDate**: The date the put-away was posted (e.g., `"2024-08-16"`).
  - **AssignedUserID**: The ID of the user assigned to this put-away (e.g., `"EMP002"`).
  - **WarehousePutAwayLines**: An array containing all lines associated with the put-away.
    - **LineNo**: The line number within the put-away (e.g., `20000`).
    - **ItemNo**: The item number associated with this line (e.g., `"ITEM002"`).
    - **VariantCode**: The variant code for the item, if any (e.g., `"VAR002"`).
    - **Quantity**: The total quantity of items in this line (e.g., `20`).
    - **QtyBase**: The base quantity (e.g., `20`).
    - **QtyToPutAway**: The quantity to be put away (e.g., `10`).
    - **QtyPutAway**: The quantity already put away (e.g., `10`).
    - **QtyOutstanding**: The outstanding quantity (e.g., `10`).
    - **UnitofMeasureCode**: The unit of measure code for the item (e.g., `"PCS"`).
    - **QtyperUnitofMeasure**: The quantity per unit of measure (e.g., `1`).
    - **NewQtyOutstanding**: The new outstanding quantity (e.g., `10`).
  - **LicensePlates**: An array containing details of the license plates associated with this put-away.
    - **LPDocumentNo**: The document number of the license plate (e.g., `"LP-000002"`).
    - **LicensePlateStatus**: The status of the license plate (e.g., `"Labeled"`).
    - **ParentLPNo**: The parent license plate number, if any (e.g., `""`).
    - **ZoneCode**: The warehouse zone code (e.g., `"ZONE02"`).
    - **LocationCode**: The location code (e.g., `"LOC02"`).
    - **BinCode**: The bin code where the license plate is located (e.g., `"BIN002"`).
    - **WhseDocumentNo**: The warehouse document number associated with the license plate (e.g., `"PA-000001"`).
    - **SystemCreatedAt**: The date and time the license plate was created (e.g., `"2024-08-16T14:22:33Z"`).
    - **SystemCreatedBy**: The user who created the license plate (e.g., `"EMP002"`).
    - **LPTotalQuantities**: The total quantities in the license plate (e.g., `20`).
    - **LPLines**: An array containing lines associated with this license plate.
      - **LineNo**: The line number within the license plate (e.g., `20000`).
      - **ItemNo**: The item number (e.g., `"ITEM002"`).
      - **VariantCode**: The variant code (e.g., `"VAR002"`).
      - **SerialNo**: The serial number of the item, if any (e.g., `"SN002"`).
      - **LotNo**: The lot number of the item, if any (e.g., `"LOT002"`).
      - **Description**: The description of the item (e.g., `"Item Description"`).
      - **Quantity**: The quantity in this line (e.g., `20`).
      - **UnitofMeasure**: The unit of measure for the item (e.g., `"PCS"`).
    - **ChildLPs**: An array containing child license plates, if any.

#### Summary
The `GetWarehousePutAway` method provides a comprehensive overview of a Warehouse Put-Away, including its lines and associated License Plates. This API is essential for warehouse management, offering detailed insights into put-away operations, enabling effective tracking and management of inventory within the system.
