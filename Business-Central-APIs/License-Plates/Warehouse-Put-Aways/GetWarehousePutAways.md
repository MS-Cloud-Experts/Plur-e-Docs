### API Documentation: GetWarehousePutAways

#### Overview
The `GetWarehousePutAways` API method retrieves a list of Warehouse Put-Aways filtered by the assigned user. This method provides detailed information about each Warehouse Put-Away, including associated lines and License Plates, ensuring that all relevant data is available for further processing or auditing.

#### Request Structure
```json
{
  "ProcessMethod": "GetWarehousePutAways",
  "Parameters": [
    {
      "WarehouseEmployee": "IVAN.LABRADOR"
    }
  ]
}
```

#### Parameters
- **WarehouseEmployee**: The ID of the user assigned to the Warehouse Put-Aways that need to be retrieved (e.g., `"EMP001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetWarehousePutAways",
  "Parameters": [
    {
       "WarehouseEmployee": "IVAN.LABRADOR"
    }
  ]
}
```

#### Example Response
```json
{
  "WarehousePutAways": [
    {
      "No": "WHSE PUTAWAY-00147",
      "LocationCode": "MAIN",
      "NoSeries": "WHSE PUTAWAY",
      "PostingDate": "0001-01-01",
      "AssignedUserID": "IVAN.LABRADOR",
      "WarehousePutAwayLines": [
        {
          "No": "WHSE PUTAWAY-00147",
          "LineNo": 10000,
          "ActionType": "Take",
          "ItemNo": "D0BDBD",
          "VariantCode": "B60W225",
          "Quantity": 6.0,
          "QtyBase": 6.0,
          "QtyToHandle": 6.0,
          "QtyHandled": 0.0,
          "QtyOutstanding": 6.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "BinCode": "MAIN",
          "ZoneCode": "REC"
        },
        {
          "No": "WHSE PUTAWAY-00147",
          "LineNo": 20000,
          "ActionType": "Place",
          "ItemNo": "D0BDBD",
          "VariantCode": "B60W225",
          "Quantity": 6.0,
          "QtyBase": 6.0,
          "QtyToHandle": 6.0,
          "QtyHandled": 0.0,
          "QtyOutstanding": 6.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0,
          "BinCode": "BACK",
          "ZoneCode": "STORAGE"
        }
      ]
    }
  ]
}
```

#### Explanation
- **WarehousePutAways**: An array of Warehouse Put-Away objects that match the assigned user ID filter.
  - **No**: The Warehouse Put-Away document number (e.g., `"WHSE PUTAWAY-00147"`).
  - **LocationCode**: The location code associated with the Warehouse Put-Away (e.g., `"MAIN"`).
  - **NoSeries**: The series number for the Warehouse Put-Away (e.g., `"WHSE PUTAWAY"`).
  - **PostingDate**: The date when the Warehouse Put-Away was posted (e.g., `"0001-01-01"`).
  - **AssignedUserID**: The ID of the user assigned to this Warehouse Put-Away (e.g., `"IVAN.LABRADOR"`).
  - **WarehousePutAwayLines**: An array of lines associated with the Warehouse Put-Away, each including details such as Line Number, Action Type, Item Number, Quantity, Unit of Measure, and Bin Code.

#### Summary
The `GetWarehousePutAways` method is designed to retrieve a filtered list of Warehouse Put-Aways based on the assigned user ID. This API is crucial for warehouse management as it allows for the tracking and auditing of Warehouse Put-Aways assigned to specific employees. The method returns detailed information, including Warehouse Put-Away lines and associated License Plates, making it easier to manage inventory and warehouse operations effectively.
