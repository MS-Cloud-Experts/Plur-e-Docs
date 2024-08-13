### API Documentation: GetLPMovements

#### Overview
The `GetLPMovements` API method retrieves the movement history of a specific License Plate (LP). This method allows you to track and review all movements associated with an LP, including quantities moved, locations, and other relevant details.

#### Request Structure
```json
{
  "ProcessMethod": "GetLPMovements",
  "Parameters": [
    {
      "LPDocumentNo": "LP-0001"
    }
  ]
}
```

#### Parameters
- **LPDocumentNo**: The License Plate document number for which the movement history is requested (e.g., `"LP-0001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetLPMovements",
  "Parameters": [
    {
      "LPDocumentNo": "LP-0001"
    }
  ]
}
```

#### Example Response
```json
{
  "LPMovements": [
    {
      "MovementNo": "MOVE-001",
      "MovementType": "Transfer",
      "LocationCode": "LOC01",
      "BinCode": "BIN01",
      "QuantityMoved": "100",
      "CurrentQuantity": "50",
      "DocumentType": "Warehouse Receipt",
      "DocumentNo": "WR-001",
      "PostingDate": "2024-08-12",
      "UserName": "user1"
    },
    {
      "MovementNo": "MOVE-002",
      "MovementType": "Adjustment",
      "LocationCode": "LOC01",
      "BinCode": "BIN02",
      "QuantityMoved": "50",
      "CurrentQuantity": "100",
      "DocumentType": "Warehouse Receipt",
      "DocumentNo": "WR-002",
      "PostingDate": "2024-08-13",
      "UserName": "user2"
    }
  ]
}
```

#### Explanation
- **MovementNo**: The unique identifier for the movement (e.g., `"MOVE-001"`).
- **MovementType**: The type of movement (e.g., `"Transfer"`).
- **LocationCode**: The location code where the movement occurred (e.g., `"LOC01"`).
- **BinCode**: The bin code associated with the movement (e.g., `"BIN01"`).
- **QuantityMoved**: The quantity moved in this specific movement (e.g., `"100"`).
- **CurrentQuantity**: The current quantity remaining after the movement (e.g., `"50"`).
- **DocumentType**: The type of document associated with the movement (e.g., `"Warehouse Receipt"`).
- **DocumentNo**: The document number associated with the movement (e.g., `"WR-001"`).
- **PostingDate**: The date when the movement was posted (e.g., `"2024-08-12"`).
- **UserName**: The name of the user who performed the movement (e.g., `"user1"`).

#### Summary
The `GetLPMovements` method provides a detailed history of all movements related to a specific License Plate. This API is crucial for tracking the flow of goods in and out of locations, ensuring accurate inventory management and traceability within the warehouse system. The method returns a comprehensive list of movements, including types, quantities, locations, and timestamps, allowing for in-depth analysis and review.