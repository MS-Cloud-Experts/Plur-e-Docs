### API Documentation: UpdateWsheReceiveLine

#### Overview
The `Update_WsheReceiveLine` API method allows updating of specific lines within a Warehouse Receipt based on the given parameters. This method is essential for adjusting the quantities to receive for items, ensuring that the Warehouse Receipt lines and their related License Plates (LPs) are updated accordingly. The method processes multiple lines in a single request and returns the updated status of the Warehouse Receipt lines.

#### Request Structure
```json
{
  "ProcessMethod": "UpdateWsheReceiveLine",
  "Parameters": [
    {
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00171",
          "LineNo": 10000,
          "ItemNo": "D0BDBD",
          "SourceNo": "SRC001",
          "QtyToReceive": 5.0
        },
        {
          "No": "WHSE REC-00171",
          "LineNo": 20000,
          "ItemNo": "D0BDBD",
          "SourceNo": "SRC001",
          "QtyToReceive": 3.0
        }
      ]
    }
  ]
}
```

#### Parameters
- **WarehouseReceiptLines**: An array of Warehouse Receipt lines that need to be updated.
  - **No**: The Warehouse Receipt document number (e.g., `"WHSE REC-00171"`).
  - **LineNo**: The line number in the Warehouse Receipt (e.g., `10000`).
  - **ItemNo**: The item number associated with the line (e.g., `"D0BDBD"`).
  - **SourceNo**: The source document number (e.g., `"SRC001"`).
  - **QtyToReceive**: The updated quantity to receive for the specific line (e.g., `5.0`).

#### Example Request
```json
{
  "ProcessMethod": "Update_WsheReceiveLine",
  "Parameters": [
    {
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00171",
          "LineNo": 10000,
          "ItemNo": "D0BDBD",
          "SourceNo": "SRC001",
          "QtyToReceive": 5.0
        },
        {
          "No": "WHSE REC-00171",
          "LineNo": 20000,
          "ItemNo": "D0BDBD",
          "SourceNo": "SRC001",
          "QtyToReceive": 3.0
        }
      ]
    }
  ]
}
```

#### Example Response
```json
{
  "WarehouseReceiptHeader": [
    {
      "No": "WHSE REC-00171",
      "WarehouseReceiptLines": [
        {
          "No": "WHSE REC-00171",
          "LineNo": 10000,
          "ItemNo": "D0BDBD",
          "BinCode": "MAIN",
          "QtyToReceive": 5.0,
          "QtyReceived": 35.0,
          "QtyOutstanding": 160.0,
          "UnitofMeasureCode": "EA",
          "LP_Received": "LP-00026-10000"
        },
        {
          "No": "WHSE REC-00171",
          "LineNo": 20000,
          "ItemNo": "D0BDBD",
          "BinCode": "MAIN",
          "QtyToReceive": 3.0,
          "QtyReceived": 1.0,
          "QtyOutstanding": 246.0,
          "UnitofMeasureCode": "EA",
          "LP_Received": ""
        }
      ],
      "LicensePlates": [
        {
          "LPDocumentNo": "LP-00026",
          "LicensePlateStatus": "Received",
          "LPTotalQuantities": 5.0,
          "LPLines": [
            {
              "LineNo": 10000,
              "ItemNo": "D0BDBD",
              "Quantity": 5.0
            }
          ]
        }
      ]
    }
  ]
}
```

#### Explanation
- **WarehouseReceiptHeader**: The main object containing details about the Warehouse Receipt after updating the lines.
  - **No**: The Warehouse Receipt document number (e.g., `"WHSE REC-00171"`).
  - **WarehouseReceiptLines**: An array containing the updated lines in the Warehouse Receipt.
    - **No**: The Warehouse Receipt number (e.g., `"WHSE REC-00171"`).
    - **LineNo**: The line number in the receipt (e.g., `10000`).
    - **ItemNo**: The item number associated with the line (e.g., `"D0BDBD"`).
    - **BinCode**: The bin where the item is located (e.g., `"MAIN"`).
    - **QtyToReceive**: The updated quantity to receive (e.g., `5.0`).
    - **QtyReceived**: The quantity already received (e.g., `35.0`).
    - **QtyOutstanding**: The remaining quantity to be received (e.g., `160.0`).
    - **UnitofMeasureCode**: The unit of measure for the item (e.g., `"EA"`).
    - **LP_Received**: The License Plate number where the items were received (e.g., `"LP-00026-10000"`).
  - **LicensePlates**: Details of the associated License Plates after updating the receipt.
    - **LPDocumentNo**: The document number of the License Plate (e.g., `"LP-00026"`).
    - **LicensePlateStatus**: The current status of the License Plate (e.g., `"Received"`).
    - **LPTotalQuantities**: The total quantities in the License Plate (e.g., `5.0`).
    - **LPLines**: Details of the lines associated with the License Plate, including item numbers and quantities (e.g., `"LineNo": 10000, "ItemNo": "D0BDBD", "Quantity": 5.0`).

#### Summary
The `Update_WsheReceiveLine` API method updates the quantities for lines within a Warehouse Receipt and returns the updated information, including License Plate (LP) details. This method ensures that the receipt lines and associated license plates are correctly updated, enabling accurate warehouse management and inventory tracking.