### API Documentation: `CheckLPLinesInUse`

#### Overview
The `CheckLPLinesInUse` API analyzes a list of items to determine if they have active License Plates (LPs) in Storage status. For each item, it provides detailed information about existing LPs, bin content, and storage status. This is particularly useful for warehouse operations that need to verify LP availability before creating new ones.

#### Request Structure
```json
{
  "ProcessMethod": "CheckLPLinesInUseFull",
  "Parameters": [
    {
      "Items": [
        {
          "ItemNo": "ITEM001",
          "VariantCode": "VAR1"
        },
        {
          "ItemNo": "ITEM002"
        }
      ]
    }
  ]
}
```

#### Parameters
- **Items**: Array of items to check
  - **ItemNo**: Item identifier (required)
  - **VariantCode**: Variant code (optional)

#### Example Request
```json
{
  "ProcessMethod": "CheckLPLinesInUseFull",
  "Parameters": [
    {
      "Items": [
        {
          "ItemNo": "1896-S"
        },
        {
          "ItemNo": "1928-S"
        }
      ]
    }
  ]
}
```

#### Example Response
```json
{
  "ItemsStatus": [
    {
      "ItemNo": "1896-S",
      "VariantCode": "",
      "HasLPInStorage": false,
      "StorageLPs": []
    },
    {
      "ItemNo": "1928-S",
      "VariantCode": "",
      "HasLPInStorage": true,
      "StorageLPs": [
        {
          "LPNo": "LP-00001",
          "Quantity": 100.0,
          "LocationCode": "LOC_TEST",
          "BinCode": "FLOOR",
          "UnitOfMeasure": "PCS",
          "SerialNo": "",
          "LotNo": "",
          "ExpirationDate": "0001-01-01",
          "ParentLPNo": "",
          "ContainsLPChild": false
        }
      ],
      "BinContentDetails": {
        "ItemNo": "1928-S",
        "VariantCode": "",
        "UnitofMeasureCode": "",
        "LocationCode": "LOC_TEST",
        "BinCode": "FLOOR",
        "TotalQtyAvailToTakeUOM": 0.0,
        "TotalQtyAvailToPick": 0.0,
        "TotalQtyAvailToPutAway": 0.0,
        "TotalQtyInBinContent": 0.0,
        "TotalQtyToTake": 0.0,
        "TotalQtyInLP": 0.0,
        "Details": []
      }
    }
  ],
  "Duration": "48 milliseconds"
}
```

#### Response Fields
- **ItemsStatus**: Array containing status information for each requested item
  - **ItemNo**: Item identifier
  - **VariantCode**: Variant code (if applicable)
  - **HasLPInStorage**: Boolean indicating if the item has any LPs in Storage status
  - **StorageLPs**: Array of LP details for the item
    - **LPNo**: License Plate identifier
    - **Quantity**: Quantity in the LP
    - **LocationCode**: Location where LP is stored
    - **BinCode**: Bin where LP is stored
    - **UnitOfMeasure**: Unit of measure used
    - **SerialNo**: Serial number (if applicable)
    - **LotNo**: Lot number (if applicable)
    - **ExpirationDate**: Expiration date (if applicable)
    - **ParentLPNo**: Parent LP number (if this LP is a child)
    - **ContainsLPChild**: Indicates if this LP has child LPs
  - **BinContentDetails**: Detailed bin content information
    - Contains various quantity measurements and availability status

#### Process Flow
1. **Input Validation**: Validates the incoming array of items
2. **Storage Check**: For each item:
   - Checks if any LPs exist in Storage status
   - Collects detailed information about existing LPs
   - Gathers bin content information
3. **Data Aggregation**: Combines all information into a comprehensive response
4. **Response Generation**: Returns detailed status information for all items

#### Common Use Cases
- Verifying LP availability before creating new LPs
- Inventory management and planning
- Warehouse operation optimization
- Preventing duplicate LP creation for items already in storage

#### Error Scenarios
```json
{
  "error": "Items array not found in parameters",
  "code": "INVALID_PARAMS",
  "timestamp": "2024-01-15T10:30:00Z"
}
```

Common error scenarios include:
- Missing or invalid Items array in request
- Invalid item numbers
- System access errors
- Invalid variant codes

#### Performance Considerations
- Response time varies based on number of items and LP complexity
- Recommended maximum of 50 items per request
- Consider pagination for large item sets

#### Summary
The `CheckLPLinesInUseFull` API is a crucial tool for warehouse management, providing comprehensive information about LP status and availability for specified items. It helps prevent duplicate LP creation and ensures efficient warehouse operations by providing detailed insights into existing LP storage status.