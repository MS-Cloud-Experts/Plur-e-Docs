### API Documentation: AdjustInventoryQuantities

#### **Overview**
The `AdjustInventoryQuantities` method allows for adjusting item quantities in the warehouse through a Warehouse Journal. This adjustment can be positive (increase) or negative (decrease). The method supports items with or without tracking (serial or lot numbers) and records all movements in the Warehouse Journal, reflecting the changes in inventory. For items with tracking, the tracking information (serial numbers, lot numbers, expiration dates) must be provided. The system processes the adjustments and posts the Warehouse Journal to ensure that inventory levels are updated correctly.

#### **Request Structure**
```json
{
  "ProcessMethod": "AdjustInventoryQuantities",
  "Parameters": [
    {
      "ItemNo": "ITEM001",
      "VariantCode": "",
      "LocationCode": "LOC001",
      "BinCode": "BIN001",
      "AdjustQty": 10,
      "TrackingInfo": []
    },
    {
      "ItemNo": "ITEM002",
      "VariantCode": "VAR001",
      "LocationCode": "LOC002",
      "BinCode": "BIN002",
      "AdjustQty": -5,
      "TrackingInfo": [
        {
          "SerialNo": "SN12345",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Quantity": 5
        }
      ]
    }
  ]
}
```

#### **Parameters**
- **ProcessMethod**: Indicates the method to invoke, in this case `"AdjustInventoryQuantities"`.
- **Parameters**: An array of objects describing the adjustments to be made in the inventory.
  - **ItemNo**: The item number associated with the inventory (e.g., `"ITEM001"`).
  - **VariantCode**: The variant code of the item, if applicable (e.g., `"VAR001"`).
  - **LocationCode**: The location where the inventory is stored (e.g., `"LOC001"`).
  - **BinCode**: The bin where the inventory is located (e.g., `"BIN001"`).
  - **AdjustQty**: The quantity to adjust (positive for an increase, negative for a decrease) (e.g., `10`).
  - **TrackingInfo**: Information related to item tracking, including serial numbers, lot numbers, and expiration dates.
    - **SerialNo**: The serial number of the item, if applicable (e.g., `"SN12345"`).
    - **LotNo**: The lot number of the item, if applicable (e.g., `"LOT001"`).
    - **ExpirationDate**: The expiration date of the item, if applicable (e.g., `"2024-12-31"`).
    - **Quantity**: The quantity related to the serial or lot number (e.g., `5`).

#### **Example Request**
```json
{
  "ProcessMethod": "AdjustInventoryQuantities",
  "Parameters": [
    {
      "ItemNo": "ITEM001",
      "VariantCode": "",
      "LocationCode": "LOC001",
      "BinCode": "BIN001",
      "AdjustQty": 10,
      "TrackingInfo": []
    },
    {
      "ItemNo": "ITEM002",
      "VariantCode": "VAR001",
      "LocationCode": "LOC002",
      "BinCode": "BIN002",
      "AdjustQty": -5,
      "TrackingInfo": [
        {
          "SerialNo": "SN12345",
          "LotNo": "LOT001",
          "ExpirationDate": "2024-12-31",
          "Quantity": 5
        }
      ]
    }
  ]
}
```

#### **Example Response**
```json
{
  "Result": "The warehouse journal was posted successfully."
}
```

#### **Explanation**
- **Result**: The message confirming that the warehouse journal was posted successfully after adjusting the inventory quantities.

#### **Summary**
The `AdjustInventoryQuantities` method allows for adjusting inventory levels in the warehouse by creating Warehouse Journal entries. The method supports both positive and negative adjustments and handles items with or without tracking information (serial numbers, lot numbers, expiration dates). After processing the adjustments, the method posts the Warehouse Journal to ensure the changes are reflected in the system.

### **Implementation Logic**
1. **Initial Validations**: 
   - Validate that the item exists in the system.
   - Ensure that the quantities to be adjusted are valid.
   - Verify that the appropriate tracking information is provided if the item has serial or lot tracking enabled.

2. **Processing Adjustments**:
   - For positive adjustments, the specified quantity is added to the item in the warehouse.
   - For negative adjustments, the specified quantity is subtracted from the item.
   - If the item has tracking information, the adjustment is made based on the provided serial number, lot number, and expiration date.

3. **Warehouse Journal Posting**:
   - After processing all adjustments, the Warehouse Journal is posted to reflect the inventory changes.
   - The system registers the movements in the Warehouse Journal and updates the inventory accordingly.

### **Additional Considerations**
- **Tracking Information**: The `TrackingInfo` array is used when serial or lot tracking is required. If the item does not require tracking, this array can be omitted.
- **Posting the Journal**: Once the adjustments are complete, the Warehouse Journal is posted to ensure the system reflects the inventory changes. This ensures that the inventory records are accurate and up-to-date.

This API provides a flexible and comprehensive way to manage inventory adjustments in a warehouse environment, with support for detailed tracking and quantity management.