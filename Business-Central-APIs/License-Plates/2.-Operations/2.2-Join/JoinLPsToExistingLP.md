### API Documentation: JoinLPsToExistingLP

The `JoinLPsToExistingLP` API allows for the consolidation of multiple License Plates (LPs) into an existing LP. This operation is essential for optimizing storage space and maintaining efficient inventory management. The process also ensures that any child LPs are transferred to the existing LP, and the original LPs are marked as "Joined" and deleted.

**Request Body:**
```json
{
  "ExistingLPDocumentNo": "LP004",
  "LPsToJoin": [
    {"LPDocumentNo": "LP001"},
    {"LPDocumentNo": "LP002"},
    {"LPDocumentNo": "LP003"}
  ]
}
```

**Parameters:**

- `ExistingLPDocumentNo` (Text): The document number of the existing LP where the selected LPs will be consolidated.
- `LPsToJoin` (Array of Objects): A list of LPs to be joined into the existing LP.
  - `LPDocumentNo` (Text): The document number of each LP that needs to be joined.

**Response Body:**
```json
{
  "ExistingLPDocumentNo": "LP004",
  "Message": "Join de LPs completado con éxito en el LP existente: LP004"
}
```

**Response Fields:**

- `ExistingLPDocumentNo` (Text): The document number of the LP where the other LPs were successfully consolidated.
- `Message` (Text): A confirmation message indicating that the operation was successfully completed.

**Example Usage:**

- **Request:**
    ```json
    {
      "ExistingLPDocumentNo": "LP004",
      "LPsToJoin": [
        {"LPDocumentNo": "LP001"},
        {"LPDocumentNo": "LP002"},
        {"LPDocumentNo": "LP003"}
      ]
    }
    ```

- **Response:**
    ```json
    {
      "ExistingLPDocumentNo": "LP004",
      "Message": "Join de LPs completado con éxito en el LP existente: LP004"
    }
    ```

**Process Flow:**

1. **Get the Existing LP:** The API retrieves the `ExistingLPDocumentNo` from the input JSON.
2. **Retrieve LPs to Join:** The API then fetches the list of LPs that need to be joined from the `LPsToJoin` array.
3. **Join LPs:** 
   - The system processes the join operation by merging the lines from the LPs in `LPsToJoin` into the `ExistingLPDocumentNo`.
   - It also transfers any child LPs associated with the original LPs to the `ExistingLPDocumentNo`.
4. **Register Movements:** The system registers the inventory movements resulting from this join operation for traceability and data integrity.
5. **Mark and Delete Original LPs:** Finally, the original LPs are marked as "Joined" and are removed from the system.

**Error Handling:**

- **Missing `LPsToJoin`:** If the `LPsToJoin` array is not found in the input JSON, the API will throw an error stating, "LPsToJoin field not found in the JSON object."
- **Invalid LP Document Number:** If any LP document number is invalid or not found, the API will throw an error specifying the missing LP.

**Dependencies:**
This API depends on the following internal procedures:
- `HelperJoin.JoinLPs`: Handles the merging of the selected LPs into the existing LP.
- `HelperJoin.RegisterJoinMovements`: Registers the movements of the LPs to ensure traceability.
- `HelperJoin.MarkAndDeleteOriginalLPs`: Marks the original LPs as "Joined" and deletes them.

**Considerations:**

- **Data Integrity:** The API ensures that the inventory movements are properly registered and that the data remains consistent after the operation.
- **Child LP Handling:** Child LPs associated with the original LPs are automatically transferred to the existing LP during the join operation.

### Summary:
The `JoinLPsToExistingLP` API provides a robust method for consolidating multiple LPs into an existing LP, streamlining inventory management, and ensuring data integrity through comprehensive tracking of all related movements.