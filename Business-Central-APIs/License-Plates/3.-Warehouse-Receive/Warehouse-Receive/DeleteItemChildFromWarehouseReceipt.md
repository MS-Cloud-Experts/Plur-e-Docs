### API Documentation: DeleteItemChildFromWarehouseReceipt

#### Overview
The `DeleteItemChildFromWarehouseReceipt` API method is designed to remove a specific item child from a License Plate (LP) associated with a Warehouse Receipt Line. This method recalculates the possible item children for the LP and provides an updated list of potential items that could be added.

#### Request Structure
```json
{
  "ProcessMethod": "DeleteItemChildFromWarehouseReceipt",
  "Parameters": [
    {
      "LP_No": "LP-0001",
      "WarehouseReceipt_No": "WR-001",
      "WarehouseReceipt_LineNo": 10000,
      "LineNo": 20000,
      "Item_Child_No": "ITEM001"
    }
  ]
}
```

#### Parameters
- **LP_No**: The License Plate number from which the item child will be removed (e.g., `"LP-0001"`).
- **WarehouseReceipt_No**: The Warehouse Receipt number associated with the LP (e.g., `"WR-001"`).
- **WarehouseReceipt_LineNo**: The line number of the Warehouse Receipt where the LP is registered (e.g., `10000`).
- **LineNo**: The line number within the LP from which the item child will be deleted (e.g., `20000`).
- **Item_Child_No**: The item number of the child item to be removed from the LP (e.g., `"ITEM001"`).

#### Example Request
```json
{
  "ProcessMethod": "DeleteItemChildFromWarehouseReceipt",
  "Parameters": [
    {
      "LP_No": "LP-0001",
      "WarehouseReceipt_No": "WR-001",
      "WarehouseReceipt_LineNo": 10000,
      "LineNo": 20000,
      "Item_Child_No": "ITEM001"
    }
  ]
}
```

#### Example Response
```json
{
  "IsProcessed": true,
  "Possible_ItemsChilds": [
    {
      "No": "WR-001",
      "LineNo": 10000,
      "ItemNo": "ITEM002",
      "Qty": 50
    },
    {
      "No": "WR-001",
      "LineNo": 10001,
      "ItemNo": "ITEM003",
      "Qty": 30
    }
  ]
}
```

#### Explanation
- **IsProcessed**: A boolean flag indicating whether the item child was successfully removed.
- **Possible_ItemsChilds**: An array of potential items that could be added as children to the LP, including their Warehouse Receipt number, line number, item number, and outstanding quantity.

#### Summary
The `DeleteItemChildFromWarehouseReceipt` method provides a controlled way to manage the removal of item children from a License Plate associated with a Warehouse Receipt Line. After the removal, the method recalculates the possible item children, ensuring accurate and updated information for further processing in the warehouse. This helps maintain the integrity of inventory records and streamlines warehouse operations.