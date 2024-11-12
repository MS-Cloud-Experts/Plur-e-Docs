### API Documentation: `CheckLPLinesInUse`

#### Overview
A lightweight API that checks if specified items have License Plates (LPs) in Storage status and returns basic quantity information. This simplified version provides essential storage status without detailed LP information.

#### Request Structure
```json
{
  "ProcessMethod": "CheckLPLinesInUse",
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

#### Example Response
```json
{
  "ItemsStatus": [
    {
      "ItemNo": "ITEM001",
      "VariantCode": "VAR1",
      "HasLPInStorage": true,
      "TotalQuantityInStorage": 150.0,
      "NumberOfLPs": 3
    },
    {
      "ItemNo": "ITEM002",
      "VariantCode": "",
      "HasLPInStorage": false,
      "TotalQuantityInStorage": 0,
      "NumberOfLPs": 0
    }
  ]
}
```

#### Response Fields
- **ItemNo**: Item identifier
- **VariantCode**: Variant code (if provided)
- **HasLPInStorage**: Boolean indicating if the item has any LPs in Storage status
- **TotalQuantityInStorage**: Total quantity of the item in Storage status LPs
- **NumberOfLPs**: Number of LPs containing this item in Storage

#### Summary
This simplified version of the API provides quick status checks for items in storage, perfect for basic inventory verification and LP availability checks. For more detailed information about LPs and bin contents, use the `CheckLPLinesInUseFull` API instead.