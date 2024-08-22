### API Documentation: AssignItemToLPWithTracking

#### Overview
The `AssignItemToLPWithTracking` API method allows for the assignment of items to a License Plate (LP) with detailed tracking information. This method is specifically designed to handle items that require tracking (e.g., serial numbers, lot numbers) during warehouse receipt processing.

#### Request Structure
```json
{
  "ProcessMethod": "AssignItemToLPWithTracking",
  "Parameters": [
    {
      "WarehouseReceiptNo": "WHSE REC-00186",
      "LPDocumentNo": "LP-00073",
      "BinCode": "MAIN",
      "Item_Child": [
        {
          "LineNo": 10000,
          "ItemNo": "K3CSODQL",
          "TotalToReceive": 2,
          "UnitofMeasureCode": "PCS",
          "SourceNo": "PO-120037",
          "SourceRefNo": 50000,
          "TrackingInfo": [
            {
              "SerialNo": "SNA001",
              "LotNo": "LOT001",
              "ExpirationDate": "2024-12-31",
              "Qty": 1
            },
            {
              "SerialNo": "SNA001",
              "LotNo": "LOT001",
              "ExpirationDate": "2024-12-31",
              "Qty": 1
            }
          ]
        }
      ]
    }
  ]
}
```

#### Parameters
- **WarehouseReceiptNo**: The warehouse receipt number associated with the operation (e.g., `"WR-0001"`).
- **LPDocumentNo**: The License Plate document number to which the item is being assigned (e.g., `"LP-0001"`).
- **BinCode**: The bin code where the item is being stored (e.g., `"BIN001"`).
- **Item_Child**: An array of items to be assigned to the LP.
  - **LineNo**: The line number in the warehouse receipt document (e.g., `10000`).
  - **ItemNo**: The item number being assigned (e.g., `"ITEM001"`).
  - **TotalToReceive**: The total quantity of the item to be received (e.g., `50`).
  - **UnitofMeasureCode**: The unit of measure code for the item (e.g., `"PCS"`).
  - **SourceNo**: The source document number associated with the item (e.g., `"PO-0001"`).
  - **SourceRefNo**: The source reference number (e.g., `1`).
  - **TrackingInfo**: An array of tracking details associated with the item.
    - **SerialNo**: The serial number of the item (e.g., `"SN001"`).
    - **LotNo**: The lot number of the item (e.g., `"LOT001"`).
    - **ExpirationDate**: The expiration date of the item (e.g., `"2024-12-31"`).
    - **Qty**: The quantity associated with this tracking detail (e.g., `50`).

#### Example Request
```json
{
  "ProcessMethod": "AssignItemToLPWithTracking",
  "Parameters": [
    {
      "WarehouseReceiptNo": "WR-0001",
      "LPDocumentNo": "LP-0001",
      "BinCode": "BIN001",
      "Item_Child": [
        {
          "LineNo": 10000,
          "ItemNo": "ITEM001",
          "TotalToReceive": 50,
          "UnitofMeasureCode": "PCS",
          "SourceNo": "PO-0001",
          "SourceRefNo": 1,
          "TrackingInfo": [
            {
              "SerialNo": "SN001",
              "LotNo": "LOT001",
              "ExpirationDate": "2024-12-31",
              "Qty": 50
            }
          ]
        }
      ]
    }
  ]
}
```

#### Example Response
```json
{
  "Message": "The LPs were created successfully.",
  "TrackingSpecificationOpen": [
    {
      "SerialNo": "SN001",
      "LotNo": "LOT001",
      "ExpirationDate": "2024-12-31",
      "Qty": 50
    }
  ],
  "LP_Pending_To_Receive": 0,
  "LP_Received": "LP-0001"
}
```

#### Explanation
- **Message**: A confirmation message indicating the success of the operation (e.g., `"The LPs were created successfully."`).
- **TrackingSpecificationOpen**: An array of open tracking specifications for the item.
  - **SerialNo**: The serial number of the item.
  - **LotNo**: The lot number of the item.
  - **ExpirationDate**: The expiration date of the item.
  - **Qty**: The quantity associated with the tracking specification.
- **LP_Pending_To_Receive**: The quantity of the item still pending to be received into the LP.
- **LP_Received**: The License Plate document number that received the items (e.g., `"LP-0001"`).

#### Summary
The `AssignItemToLPWithTracking` API method provides a streamlined approach to assigning items with detailed tracking information to a License Plate during the warehouse receipt process. It ensures that all tracking details are accurately captured and associated with the LP, facilitating efficient inventory management and traceability.