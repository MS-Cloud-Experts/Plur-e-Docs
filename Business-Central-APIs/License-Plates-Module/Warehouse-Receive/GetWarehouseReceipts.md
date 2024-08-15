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
- **WarehouseEmployee**: The ID of the user assigned to the Warehouse Receipts that need to be retrieved (e.g., `"EMP001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWarehouseReceipts",
  "Parameters": [
    {
      "WarehouseEmployee": "EMP001"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehouseReceipts": [
    {
      "No": "WHSE REC-00170",
      "LocationCode": "MAIN",
      "NoSeries": "WHSE REC",
      "PostingDate": "2024-08-13",
      "AssignedUserID": "IVAN.LABRADOR",
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00170",
          "LineNo": 10000,
          "ItemNo": "K4KODRIFR",
          "BinCode": "MAIN",
          "VariantCode": "007001",
          "Quantity": 200.0,
          "QtyBase": 200.0,
          "QtyToReceive": 0.0,
          "QtyReceived": 0.0,
          "QtyOutstanding": 200.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 200.0,
          "TrackingSpecificationOpen": [],
          "LP_Pending_To_Receive": 200.0,
          "LP_Received": ""
        },
        {
          "No": "WHSE REC-00170",
          "LineNo": 20000,
          "ItemNo": "K4KODRIFR",
          "BinCode": "MAIN",
          "VariantCode": "007002",
          "Quantity": 300.0,
          "QtyBase": 300.0,
          "QtyToReceive": 0.0,
          "QtyReceived": 0.0,
          "QtyOutstanding": 300.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 300.0,
          "TrackingSpecificationOpen": [],
          "LP_Pending_To_Receive": 300.0,
          "LP_Received": ""
        },
        {
          "No": "WHSE REC-00170",
          "LineNo": 30000,
          "ItemNo": "K4KOMOTOX",
          "BinCode": "MAIN",
          "VariantCode": "006003",
          "Quantity": 150.0,
          "QtyBase": 150.0,
          "QtyToReceive": 0.0,
          "QtyReceived": 0.0,
          "QtyOutstanding": 150.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 150.0,
          "TrackingSpecificationOpen": [],
          "LP_Pending_To_Receive": 150.0,
          "LP_Received": ""
        },
        {
          "No": "WHSE REC-00170",
          "LineNo": 40000,
          "ItemNo": "K4KOMOTOX",
          "BinCode": "MAIN",
          "VariantCode": "008001",
          "Quantity": 200.0,
          "QtyBase": 200.0,
          "QtyToReceive": 0.0,
          "QtyReceived": 0.0,
          "QtyOutstanding": 200.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 200.0,
          "TrackingSpecificationOpen": [],
          "LP_Pending_To_Receive": 200.0,
          "LP_Received": ""
        }
      ]
    },
    {
      "No": "WHSE REC-00171",
      "LocationCode": "MAIN",
      "NoSeries": "WHSE REC",
      "PostingDate": "2024-08-13",
      "AssignedUserID": "IVAN.LABRADOR",
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00171",
          "LineNo": 10000,
          "ItemNo": "D0BDBD",
          "BinCode": "MAIN",
          "VariantCode": "B60W225",
          "Quantity": 200.0,
          "QtyBase": 200.0,
          "QtyToReceive": 6.0,
          "QtyReceived": 29.0,
          "QtyOutstanding": 171.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 165.0,
          "TrackingSpecificationOpen": [],
          "LP_Pending_To_Receive": 165.0,
          "LP_Received": "LP-00020-10000|LP-00021-10000"
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
          "QtyReceived": 1.0,
          "QtyOutstanding": 249.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "NewQtyOutstanding": 249.0,
          "TrackingSpecificationOpen": [],
          "LP_Pending_To_Receive": 249.0,
          "LP_Received": ""
        }
      ]
    }
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

#### Summary
The `GetWarehouseReceipts` method is designed to retrieve a filtered list of Warehouse Receipts based on the assigned user ID. This API is crucial for warehouse management as it allows for the tracking and auditing of Warehouse Receipts assigned to specific employees. The method returns detailed information, including Warehouse Receipt lines and associated License Plates, making it easier to manage inventory and warehouse operations effectively.