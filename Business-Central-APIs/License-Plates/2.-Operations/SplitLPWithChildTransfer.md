### API Documentation: SplitLPWithChildTransfer

#### Overview
The `SplitLPWithChildTransfer` API method enables the splitting of a License Plate (LP) and the transfer of its child LP to a new parent LP. This operation ensures that the child LP is correctly reassigned, and the original LP is deleted if it no longer has any children or lines associated with it.

#### Request Structure
```json
{
  "ProcessMethod": "SplitLPWithChildTransfer",
  "Parameters": [
    {
      "LPDocumentNo": "LP03",
      "LPChildToTransfer": {
        "ChildLPDocumentNo": "LP02",
        "NewParentLPNo": "LP04"
      }
    }
  ]
}
```

#### Parameters
- **LPDocumentNo**: The original LP number that will be split and from which the child LP will be transferred (e.g., `"LP03"`).
- **LPChildToTransfer**: A JSON object that specifies the child LP to transfer and the new parent LP.
  - **ChildLPDocumentNo**: The LP number of the child that will be transferred (e.g., `"LP02"`).
  - **NewParentLPNo**: The LP number of the new parent LP to which the child will be transferred (e.g., `"LP04"`). If this LP does not exist, it will be created.

#### Example Request
```json
{
  "ProcessMethod": "SplitLPWithChildTransfer",
  "Parameters": [
    {
      "LPDocumentNo": "LP03",
      "LPChildToTransfer": {
        "ChildLPDocumentNo": "LP02",
        "NewParentLPNo": "LP04"
      }
    }
  ]
}
```

#### Example Response
```json
{
  "Message": "Split con transferencia de LP hijo completado con éxito."
}
```

#### Explanation
- **Message**: A confirmation message indicating that the LP split and child transfer operation was successful.

#### Process Flow
1. **Validate Original LP**: The system verifies that the original LP (`LP03`) exists.
2. **Process Child LP Transfer**: 
   - The system checks if the child LP (`LP02`) needs to be transferred to a new parent LP (`LP04`).
   - If the new parent LP does not exist, it is created.
   - The child LP (`LP02`) is then reassigned to the new parent LP (`LP04`).
3. **Delete Child Relation**: If the child LP is successfully transferred, the relationship between the original LP (`LP03`) and the child LP (`LP02`) is deleted.
4. **Check and Delete Original LP**: 
   - The system checks if the original LP (`LP03`) has any remaining children or lines.
   - If it does not, the original LP (`LP03`) is deleted.

#### Considerations
- **Integrity of Inventory**: The API ensures that inventory integrity is maintained by validating that child LPs are correctly reassigned and that no orphaned LPs remain in the system.
- **Automatic Creation of New Parent LP**: If the new parent LP specified does not exist, the system will automatically create it, ensuring seamless operation.
- **Restrictions**: The system will only delete the original LP if it has no remaining children or lines, preventing accidental loss of inventory data.

#### Summary
The `SplitLPWithChildTransfer` API is designed to facilitate the splitting of an LP and the transfer of its child LP to a new parent LP. This method is essential for maintaining accurate inventory tracking in complex warehouse environments where LPs may need to be reorganized. The API handles the creation of new parent LPs, reassignment of child LPs, and cleanup of old LPs, ensuring that the system remains consistent and accurate.