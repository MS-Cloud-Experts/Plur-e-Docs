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

#### Parameters
- **Items**: Array of items to check
  - **ItemNo**: Item identifier (required)
  - **VariantCode**: Variant code (optional)

#### Example Response
```json
{
  "ItemsStatus": [
    {
      "ItemNo": "1896-S",
      "VariantCode": "",
      "HasLPInStorage": false,
      "TotalQuantityInStorage": 0,
      "NumberOfLPs": 0
    },
    {
      "ItemNo": "1928-S",
      "VariantCode": "",
      "HasLPInStorage": true,
      "TotalQuantityInStorage": 100.0,
      "NumberOfLPs": 1
    }
  ],
  "Duration": "97 milliseconds"
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