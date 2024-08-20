### API Documentation: `GetItemTracking`

#### Overview
The `GetItemTracking` API method retrieves detailed tracking information about a specific item based on provided parameters. It processes the source details and returns a JSON object containing the item tracking information, which includes various tracking configurations such as serial number tracking, lot tracking, and package tracking.

#### Request Structure
```json
{
  "ProcessMethod": "GetItemTracking",
  "Parameters": [
    {
      "SourceType": 1,
      "SourceSubtype": 0,
      "SourceNo": "ITEM123",
      "SourceRefNo": 100
    }
  ]
}
```

#### Parameters
- **SourceType**: The type of the source for which the item tracking information is requested. It is an integer representing different source types (e.g., `1` for sales order, `2` for purchase order).
- **SourceSubtype**: The subtype of the source, which can be used to further categorize the source type. It is an integer value.
- **SourceNo**: The unique identifier of the source (e.g., the item number). This is a string with a maximum length of 20 characters.
- **SourceRefNo**: A reference number associated with the source, usually representing the line number of the source document. This is an integer.

#### Example Request
```json
{
  "ProcessMethod": "GetItemTracking",
  "Parameters": [
    {
      "SourceType": 1,
      "SourceSubtype": 0,
      "SourceNo": "ITEM123",
      "SourceRefNo": 100
    }
  ]
}
```

#### Example Response
```json
{
  "ItemTrackingJO": {
    "Code": "TRACK001",
    "Description": "Tracking for Item 123",
    "WarrantyDateFormula": "1Y",
    "ManWarrantyDateEntryReqd": true,
    "ManExpirDateEntryReqd": false,
    "StrictExpirationPosting": true,
    "UseExpirationDates": true,
    "SNSpecificTracking": false,
    "SNInfoInboundMustExist": false,
    "SNInfoOutboundMustExist": true,
    "SNWarehouseTracking": false,
    "SNPurchaseInboundTracking": true,
    "SNPurchaseOutboundTracking": false,
    "SNSalesInboundTracking": false,
    "SNSalesOutboundTracking": true,
    "SNPosAdjmtInbTracking": false,
    "SNPosAdjmtOutbTracking": false,
    "SNNegAdjmtInbTracking": true,
    "SNNegAdjmtOutbTracking": false,
    "SNTransferTracking": true,
    "SNManufInboundTracking": false,
    "SNManufOutboundTracking": true,
    "SNAssemblyInboundTracking": false,
    "SNAssemblyOutboundTracking": false,
    "CreateSNInfoOnPosting": true,
    "LotSpecificTracking": false,
    "LotInfoInboundMustExist": true,
    "LotInfoOutboundMustExist": false,
    "LotWarehouseTracking": true,
    "LotPurchaseInboundTracking": false,
    "LotPurchaseOutboundTracking": true,
    "LotSalesInboundTracking": false,
    "LotSalesOutboundTracking": false,
    "LotPosAdjmtInbTracking": true,
    "LotPosAdjmtOutbTracking": false,
    "LotNegAdjmtInbTracking": false,
    "LotNegAdjmtOutbTracking": true,
    "LotTransferTracking": true,
    "LotManufInboundTracking": false,
    "LotManufOutboundTracking": false,
    "LotAssemblyInboundTracking": true,
    "LotAssemblyOutboundTracking": false,
    "CreateLotNoInfoOnPosting": true,
    "PackageSpecificTracking": false,
    "PackageWarehouseTracking": true,
    "PackageInfoInbMustExist": true,
    "PackageInfoOutbMustExist": false,
    "PackagePurchaseInbTracking": false,
    "PackagePurchOutbTracking": true,
    "PackageSalesInboundTracking": false,
    "PackageSalesOutbTracking": true,
    "PackagePosInbTracking": true,
    "PackagePosOutbTracking": false,
    "PackageNegInbTracking": true,
    "PackageNegOutbTracking": false,
    "PackageTransferTracking": true,
    "PackageManufInbTracking": false,
    "PackageManufOutbTracking": true,
    "PackageAssemblyInbTracking": false,
    "PackageAssemblyOutTracking": true
  }
}
```

#### Explanation
- **Code**: The code representing the item tracking configuration.
- **Description**: A text description of the item tracking.
- **WarrantyDateFormula**: The formula used to calculate the warranty date for the item.
- **ManWarrantyDateEntryReqd**: Indicates if the manual warranty date entry is required.
- **ManExpirDateEntryReqd**: Indicates if the manual expiration date entry is required.
- **StrictExpirationPosting**: Indicates if strict expiration posting is enforced.
- **UseExpirationDates**: Indicates if expiration dates are used for tracking.
- **SNSpecificTracking**: Indicates if serial number-specific tracking is enabled.
- **SNInfoInboundMustExist**: Indicates if serial number information must exist for inbound transactions.
- **SNInfoOutboundMustExist**: Indicates if serial number information must exist for outbound transactions.
- **SNWarehouseTracking**: Indicates if warehouse tracking by serial number is enabled.
- **SNPurchaseInboundTracking**: Indicates if serial number tracking for purchase inbound is enabled.
- **SNPurchaseOutboundTracking**: Indicates if serial number tracking for purchase outbound is enabled.
- **SNSalesInboundTracking**: Indicates if serial number tracking for sales inbound is enabled.
- **SNSalesOutboundTracking**: Indicates if serial number tracking for sales outbound is enabled.
- **SNPosAdjmtInbTracking**: Indicates if serial number tracking for positive adjustment inbound is enabled.
- **SNPosAdjmtOutbTracking**: Indicates if serial number tracking for positive adjustment outbound is enabled.
- **SNNegAdjmtInbTracking**: Indicates if serial number tracking for negative adjustment inbound is enabled.
- **SNNegAdjmtOutbTracking**: Indicates if serial number tracking for negative adjustment outbound is enabled.
- **SNTransferTracking**: Indicates if serial number tracking for transfers is enabled.
- **SNManufInboundTracking**: Indicates if serial number tracking for manufacturing inbound is enabled.
- **SNManufOutboundTracking**: Indicates if serial number tracking for manufacturing outbound is enabled.
- **SNAssemblyInboundTracking**: Indicates if serial number tracking for assembly inbound is enabled.
- **SNAssemblyOutboundTracking**: Indicates if serial number tracking for assembly outbound is enabled.
- **CreateSNInfoOnPosting**: Indicates if serial number information should be created during posting.
- **LotSpecificTracking**: Indicates if lot-specific tracking is enabled.
- **LotInfoInboundMustExist**: Indicates if lot information must exist for inbound transactions.
- **LotInfoOutboundMustExist**: Indicates if lot information must exist for outbound transactions.
- **LotWarehouseTracking**: Indicates if warehouse tracking by lot number is enabled.
- **LotPurchaseInboundTracking**: Indicates if lot tracking for purchase inbound is enabled.
- **LotPurchaseOutboundTracking**: Indicates if lot tracking for purchase outbound is enabled.
- **LotSalesInboundTracking**: Indicates if lot tracking for sales inbound is enabled.
- **LotSalesOutboundTracking**: Indicates if lot tracking for sales outbound is enabled.
- **LotPosAdjmtInbTracking**: Indicates if lot tracking for positive adjustment inbound is enabled.
- **LotPosAdjmtOutbTracking**: Indicates if lot tracking for positive adjustment outbound is enabled.
- **LotNegAdjmtInbTracking**: Indicates if lot tracking for negative adjustment inbound is enabled.
- **LotNegAdjmtOutbTracking**: Indicates if lot tracking for negative adjustment outbound is enabled.
- **LotTransferTracking**: Indicates if lot tracking for transfers is enabled.
- **LotManufInboundTracking**: Indicates if lot tracking for manufacturing inbound is enabled.
- **LotManufOutboundTracking**: Indicates if lot tracking for manufacturing outbound is enabled.
- **LotAssemblyInboundTracking**: Indicates if lot tracking for assembly inbound is enabled.
- **LotAssemblyOutboundTracking**: Indicates if lot tracking for assembly outbound is enabled.
- **CreateLotNoInfoOnPosting**: Indicates if lot number information should be created during posting.
- **PackageSpecificTracking**: Indicates if package-specific tracking is enabled.
- **PackageWarehouseTracking**: Indicates if warehouse tracking by package is enabled.
- **PackageInfoInbMustExist**: Indicates if package information must exist for inbound transactions.
- **PackageInfoOutbMustExist**: Indicates if package information must exist for outbound transactions.
- **PackagePurchaseInbTracking**: Indicates if package tracking for purchase inbound is enabled.
- **PackagePurchOutbTracking**: Indicates if package tracking for purchase outbound is enabled.
- **PackageSalesInboundTracking**: Indicates if package tracking for sales inbound is enabled.
- **PackageSalesOutbTracking**: Indicates if package tracking for sales outbound is enabled.
- **PackagePosInbTracking**: Indicates if package tracking for positive adjustment inbound is enabled.
- **PackagePosOutbTracking**: Indicates if package tracking for positive adjustment outbound is enabled.
- **PackageNegInbTracking**: Indicates if package tracking for negative adjustment inbound is enabled.
- **PackageNegOutbTracking**: Indicates if package tracking for negative adjustment outbound is enabled.
- **PackageTransferTracking**: Indicates if package tracking for transfers is enabled.
- **PackageManufInbTracking**: Indicates if