### API Documentation: GetRegisteredPutAways

#### Overview
The `GetRegisteredPutAways` API method retrieves a list of Registered Put-Aways filtered by the assigned user. This method provides detailed information about each Registered Put-Away, including associated lines, ensuring that all relevant data is available for further processing or auditing.

#### Request Structure
```json
{
  "ProcessMethod": "GetRegisteredPutAways",
  "Parameters": [
    {
      "WarehouseEmployee": "IVAN.LABRADOR"
    }
  ]
}
```

#### Parameters
- **WarehouseEmployee**: The ID of the user assigned to the Registered Put-Aways that need to be retrieved (e.g., `"EMP001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetRegisteredPutAways",
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
  "RegisteredPutAways": [
    {
      "No": "REG PUTAWAY-00146",
      "LocationCode": "MAIN",
      "NoSeries": "REG PUTAWAY",
      "RegisteringDate": "2024-08-15",
      "AssignedUserID": "IVAN.LABRADOR",
      "RegisteredPutAwayLines": [
        {
          "No": "REG PUTAWAY-00146",
          "LineNo": 10000,
          "ItemNo": "D0BDBD",
          "VariantCode": "B60W225",
          "Quantity": 6.0,
          "QtyBase": 6.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0
        },
        {
          "No": "REG PUTAWAY-00146",
          "LineNo": 20000,
          "ItemNo": "D0BDBD",
          "VariantCode": "B60W225",
          "Quantity": 6.0,
          "QtyBase": 6.0,
          "UnitofMeasureCode": "EA",
          "QtyperUnitofMeasure": 1.0
        }
      ]
    }
  ]
}
```

#### Explanation
- **RegisteredPutAways**: An array of Registered Put-Away objects that match the assigned user ID filter.
  - **No**: The Registered Put-Away document number (e.g., `"REG PUTAWAY-00146"`).
  - **LocationCode**: The location code associated with the Registered Put-Away (e.g., `"MAIN"`).
  - **NoSeries**: The series number for the Registered Put-Away (e.g., `"REG PUTAWAY"`).
  - **RegisteringDate**: The date when the Registered Put-Away was recorded (e.g., `"2024-08-15"`).
  - **AssignedUserID**: The ID of the user assigned to this Registered Put-Away (e.g., `"IVAN.LABRADOR"`).
  - **RegisteredPutAwayLines**: An array of lines associated with the Registered Put-Away, each including details such as Line Number, Item Number, Quantity, and Unit of Measure.

#### Summary
The `GetRegisteredPutAways` method is designed to retrieve a filtered list of Registered Put-Aways based on the assigned user ID. This API is crucial for warehouse management as it allows for the tracking and auditing of Registered Put-Aways assigned to specific employees. The method returns detailed information, including Registered Put-Away lines, making it easier to manage inventory and warehouse operations effectively.

