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
  "Duration": "131 milliseconds"
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