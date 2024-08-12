### API Documentation: DeleteLPChildFromWarehouseReceipt

#### Overview
The `DeleteLPChildFromWarehouseReceipt` API method allows for the removal of child License Plates (LP) from a parent LP associated with a Warehouse Receipt. After the specified child LPs are deleted, the method calculates and returns the remaining possible child LPs that can be linked to the parent LP.

#### Request Structure
```json
{
  "ProcessMethod": "DeleteLPChildFromWarehouseReceipt",
  "Parameters": [
    {
      "LP_No": "LP-0001",
      "WarehouseReceipt_No": "WR-001",
      "LP_Child": [
        { "LP_Child_No": "LP-CHILD-001" },
        { "LP_Child_No": "LP-CHILD-002" }
      ]
    }
  ]
}
```

#### Parameters
- **LP_No**: The parent License Plate number from which child LPs will be removed (e.g., `"LP-0001"`).
- **WarehouseReceipt_No**: The Warehouse Receipt number associated with the LP (e.g., `"WR-001"`).
- **LP_Child**: An array of child LPs to be removed, where each object contains:
  - **LP_Child_No**: The License Plate number of the child LP to be removed (e.g., `"LP-CHILD-001"`).

#### Example Request
```json
{
  "ProcessMethod": "DeleteLPChildFromWarehouseReceipt",
  "Parameters": [
    {
      "LP_No": "LP-0001",
      "WarehouseReceipt_No": "WR-001",
      "LP_Child": [
        { "LP_Child_No": "LP-CHILD-001" },
        { "LP_Child_No": "LP-CHILD-002" }
      ]
    }
  ]
}
```

#### Example Response
```json
{
  "IsProcessed": true,
  "Remnant_LPChilds": [
    { "LP_Child_No": "LP-CHILD-003" },
    { "LP_Child_No": "LP-CHILD-004" }
  ]
}
```

#### Explanation
- **IsProcessed**: A boolean flag indicating whether the child LPs were successfully removed.
- **Remnant_LPChilds**: An array of the remaining possible child LPs that could be linked to the parent LP, including their License Plate numbers.

#### Summary
The `DeleteLPChildFromWarehouseReceipt` method provides a streamlined way to manage the removal of child License Plates from a parent LP associated with a Warehouse Receipt. After the removal process, the method recalculates and provides a list of potential child LPs that could be linked to the parent LP. This functionality is essential for maintaining accurate and up-to-date relationships between License Plates in a warehouse management system.