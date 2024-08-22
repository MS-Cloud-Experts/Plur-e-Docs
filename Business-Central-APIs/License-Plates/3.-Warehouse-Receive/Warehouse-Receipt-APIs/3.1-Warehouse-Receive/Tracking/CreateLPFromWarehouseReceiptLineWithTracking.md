Aquí tienes un ejemplo didáctico con tres unidades a recibir:

### API Documentation: CreateLPFromWarehouseReceiptLineWithTracking

#### Request Structure
```json
{
  "ProcessMethod": "CreateLPFromWarehouseReceiptLineWithTracking",
  "Parameters": [
    {
      "No": "WHSE REC-0001",
      "ItemNo": "ITEM-001",
      "BinCode": "BIN-01",
      "LineNo": 10000,
      "UnitofMeasureCode": "PCS",
      "TotalToReceive": 3,
      "PackUnitUoM": "BOX",
      "TrackingInfo": [
        {
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN002",
          "LotNo": "LOT002",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN003",
          "LotNo": "LOT003",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        }
      ]
    }
  ]
}
```

#### Example Request
```json
{
  "ProcessMethod": "CreateLPFromWarehouseReceiptLineWithTracking",
  "Parameters": [
    {
      "No": "WHSE REC-0001",
      "ItemNo": "ITEM-001",
      "BinCode": "BIN-01",
      "LineNo": 10000,
      "UnitofMeasureCode": "PCS",
      "TotalToReceive": 3,
      "PackUnitUoM": "BOX",
      "TrackingInfo": [
        {
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN002",
          "LotNo": "LOT002",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        },
        {
          "SerialNo": "SN003",
          "LotNo": "LOT003",
          "ExpirationDate": "2024-12-31",
          "Qty": 1
        }
      ]
    }
  ]
}
```

Output: 
```json
{
  "WarehouseReceiptNo": "WHSE REC-00186",
  "ItemNo": "K3CSODQL",
  "LineNo": 10000,
  "VariantCode": "NMEDXXX",
  "TrackingSpecificationOpen": [
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN001",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN001",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN002",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN001",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN002",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K3CSODQL",
      "VariantCode": "NMEDXXX",
      "Description": "",
      "SerialNo": "SN003",
      "LotNo": "",
      "SourceID": "PO-120037",
      "LocationCode": "MAIN",
      "SourceRefNo": 50000,
      "Qty": 1.0,
      "UnitofMeasureCode": 1.0,
      "QtytoHandleBase": 1.0,
      "QtytoInvoiceBase": 1.0,
      "ExpirationDate": "0001-01-01"
    }
  ],
  "LP_Pending_To_Receive": 0.0,
  "LP_Received": "LP-00063-10000|LP-00063-20000|LP-00063-30000|LP-00063-40000|LP-00063-50000|LP-00063-60000|LP-00063-70000|LP-00063-80000|LP-00063-90000|LP-00063-100000|LP-00063-110000",
  "Message": "The LPs were created successfully with tracking.",
  "Duration": "334 milliseconds"
}
```

#### Explanation
- **WarehouseReceiptNo**: `"WHSE REC-0001"` - The warehouse receipt number for which the LPs are being created.
- **ItemNo**: `"ITEM-001"` - The item number associated with the warehouse receipt line.
- **BinCode**: `"BIN-01"` - The bin code where the items are stored.
- **LineNo**: `10000` - The line number of the warehouse receipt.
- **UnitofMeasureCode**: `"PCS"` - The unit of measure code for the items.
- **TotalToReceive**: `3` - The total quantity of items to receive.
- **PackUnitUoM**: `"BOX"` - The packing unit of measure.
- **TrackingInfo**: An array containing tracking information for the items, where each item is represented with a unique `SerialNo`, `LotNo`, and `ExpirationDate`. Each entry also includes the `Qty` for that specific item.


#### Summary
In this simplified example, the API handles a case where three units of an item are being received. Each unit has a unique serial number and lot number, ensuring proper tracking and identification within the warehouse. The `TrackingInfo` array contains individual entries for each unit, each specifying a quantity of 1, making the process straightforward and easy to understand. This approach is ideal for managing serialized inventory where each item needs to be tracked individually.