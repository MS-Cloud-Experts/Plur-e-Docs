### API Documentation: GetWarehouseReceipts

#### Overview
The `GetWarehouseReceipts` API method retrieves a list of Warehouse Receipts filtered by the assigned user. This method provides detailed information about each Warehouse Receipt, including associated lines and License Plates, ensuring that all relevant data is available for further processing or auditing.

#### Request Structure
```json
{
  "ProcessMethod": "GetWarehouseReceipts",
  "Parameters": [
    {
      "WarehouseEmployee": "IVAN.LABRADOR"
    }
  ]
}
```

#### Parameters
- **assigned_user_id**: The ID of the user assigned to the Warehouse Receipts that need to be retrieved (e.g., `"EMP001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWarehouseReceipts",
  "Parameters": [
    {
      "assigned_user_id": "EMP001"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehouseReceipts": [
    {
      "No": "WR-0001",
      "LocationCode": "LOC01",
      "NoSeries": "WR-SERIES",
      "PostingDate": "2024-08-14",
      "AssignedUserID": "EMP001",
      "WarehouseReceiptLines": [
        {
          "LineNo": 10000,
          "ItemNo": "ITEM001",
          "Quantity": 50,
          "UnitOfMeasureCode": "PCS"
        },
        ...
      ],
      "LicensePlates": [
        {
          "LPDocumentNo": "LP-0001",
          "LocationCode": "LOC01",
          "BinCode": "BIN01",
          "Status": "Received"
        },
        ...
      ]
    },
    ...
  ]
}
```

#### Explanation
- **WarehouseReceipts**: An array of Warehouse Receipt objects that match the assigned user ID filter.
  - **No**: The Warehouse Receipt document number (e.g., `"WR-0001"`).
  - **LocationCode**: The location code associated with the Warehouse Receipt (e.g., `"LOC01"`).
  - **NoSeries**: The series number for the Warehouse Receipt (e.g., `"WR-SERIES"`).
  - **PostingDate**: The date when the Warehouse Receipt was posted (e.g., `"2024-08-14"`).
  - **AssignedUserID**: The ID of the user assigned to this Warehouse Receipt (e.g., `"EMP001"`).
  - **WarehouseReceiptLines**: An array of lines associated with the Warehouse Receipt, each including details such as Line Number, Item Number, Quantity, and Unit of Measure.
  - **LicensePlates**: An array of License Plates associated with the Warehouse Receipt, each including details such as LP Document Number, Location Code, Bin Code, and Status.

#### Summary
The `GetWarehouseReceipts` method is designed to retrieve a filtered list of Warehouse Receipts based on the assigned user ID. This API is crucial for warehouse management as it allows for the tracking and auditing of Warehouse Receipts assigned to specific employees. The method returns detailed information, including Warehouse Receipt lines and associated License Plates, making it easier to manage inventory and warehouse operations effectively.