### API Documentation: GetRegisteredPutAway

#### Overview
The `GetRegisteredPutAway` API method retrieves detailed information about a specific Registered Warehouse Put-Away, including its associated lines and related License Plates (LPs). This method is essential for tracking completed warehouse put-away operations, providing users with a structured JSON response that includes all relevant details.

#### Request Structure
```json
{
  "ProcessMethod": "GetRegisteredPutAway",
  "Parameters": [
    {
      "RegisteredPutAwayNo": "RP-000001",
      "WarehouseEmployee": "EMP002"
    }
  ]
}
```

#### Parameters
- **RegisteredPutAwayNo**: The Registered Put-Away document number to retrieve (e.g., `"RP-000001"`).
- **WarehouseEmployee**: The ID of the warehouse employee associated with the put-away (e.g., `"EMP002"`).

#### Example Request
```json
{
  "ProcessMethod": "GetRegisteredPutAway",
  "Parameters": [
    {
      "RegisteredPutAwayNo": "RP-000001",
      "WarehouseEmployee": "EMP002"
    }
  ]
}
```

#### Example Response
```json
{
  "RegisteredPutAwayHeader": [
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
      ],
      "LicensePlates": [
        [
          {
            "LPDocumentNo": "LP-00020",
            "LicensePlateStatus": "Stored",
            "ParentLPNo": "",
            "ZoneCode": "STORAGE",
            "LocationCode": "MAIN",
            "BinCode": "BACK",
            "WhseDocumentNo": "WHSE REC-00171",
            "SystemCreatedAt": "2024-08-15T13:47:05.7170000Z",
            "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
            "LPTotalQuantities": 3.0,
            "LPLines": [
              {
                "LineNo": 10000,
                "ItemNo": "D0BDBD",
                "VariantCode": "B60W225",
                "SerialNo": "",
                "LotNo": "",
                "Description": "",
                "Quantity": 3.0,
                "UnitofMeasure": "EA"
              }
            ],
            "ChildLPs": []
          },
          {
            "LPDocumentNo": "LP-00021",
            "LicensePlateStatus": "Stored",
            "ParentLPNo": "",
            "ZoneCode": "STORAGE",
            "LocationCode": "MAIN",
            "BinCode": "BACK",
            "WhseDocumentNo": "WHSE REC-00171",
            "SystemCreatedAt": "2024-08-15T13:48:44.1670000Z",
            "SystemCreatedBy": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
            "LPTotalQuantities": 8.0,
            "LPLines": [
              {
                "LineNo": 10000,
                "ItemNo": "D0BDBD",
                "VariantCode": "B60W225",
                "SerialNo": "",
                "LotNo": "",
                "Description": "",
                "Quantity": 3.0,
                "UnitofMeasure": "EA"
              },
              {
                "LineNo": 20000,
                "ItemNo": "D0BDBD",
                "VariantCode": "B60W225",
                "SerialNo": "",
                "LotNo": "",
                "Description": "225X60CM",
                "Quantity": 5.0,
                "UnitofMeasure": "EA"
              }
            ],
            "ChildLPs": []
          }
        ]
      ]
    }
  ]
}
```

#### Explanation
- **RegisteredPutAwayHeader**: The main object containing all details about the registered put-away.
  - **No**: The Registered Put-Away number (e.g., `"RP-000001"`).
  - **LocationCode**: The code of the warehouse location (e.g., `"LOC02"`).
  - **NoSeries**: The number series used for the put-away (e.g., `"RPA-001"`).
  - **RegisteringDate**: The date the put-away was registered (e.g., `"2024-08-16"`).
  - **AssignedUserID**: The ID of the user assigned to this put-away (e.g., `"EMP002"`).
  - **RegisteredPutAwayLines**: An array containing all lines associated with the registered put-away.
    - **LineNo**: The line number within the registered put-away (e.g., `20000`).
    - **ItemNo**: The item number associated with this line (e.g., `"ITEM002"`).
    - **VariantCode**: The variant code for the item, if any (e.g., `"VAR002"`).
    - **Quantity**: The total quantity of items in this line (e.g., `20`).
    - **QtyBase**: The base quantity (e.g., `20`).
    - **QtyPutAway**: The quantity that was put away (e.g., `10`).
    - **QtyPutAwayBase**: The base quantity that was put away (e.g., `10`).
    - **QtyOutstanding**: The outstanding quantity (e.g., `10`).
    - **UnitofMeasureCode**: The unit of measure code for the item (e.g., `"PCS"`).
    - **QtyperUnitofMeasure**: The quantity per unit of measure (e.g., `1`).
  - **LicensePlates**: An array containing details of the license plates associated with this registered put-away.
    - **LPDocumentNo**: The document number of the license plate (e.g., `"LP-000002"`).
    - **LicensePlateStatus**: The status of the license plate (e.g., `"Stored"`).
    - **ParentLPNo**: The parent license plate number, if any (e.g., `""`).
    - **ZoneCode**: The warehouse zone code (e.g., `"ZONE02"`).
    - **LocationCode**: The location code (e.g., `"LOC02"`).
    - **BinCode**: The bin code where the license plate is located (e.g., `"BIN002"`).
    - **WhseDocumentNo**: The warehouse document number associated with the license plate (e.g., `"RP-000001"`).
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
The `GetRegisteredPutAway` method provides a comprehensive overview of a Registered Put-Away, including its lines and associated License Plates. This API is crucial for warehouse management, offering detailed insights into completed put-away operations, enabling effective tracking and management of inventory within the system.
