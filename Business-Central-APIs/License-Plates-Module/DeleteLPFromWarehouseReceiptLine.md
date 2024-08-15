### API Documentation: DeleteLPFromWarehouseReceiptLine

#### Overview
The `DeleteLPFromWarehouseReceiptLine` API method deletes a specified License Plate (LP) that is associated with a warehouse receipt line. This method ensures that the LP exists, verifies its status, and confirms its assignment to a warehouse receipt before performing the deletion.

#### Request Structure
```json
{
  "ProcessMethod": "DeleteLPFromWarehouseReceiptLine",
  "Parameters": [
    {
      "LPDocumentNo": "LP-0001"
    }
  ]
}
```

#### Parameters
- **LPDocumentNo**: The document number of the License Plate to be deleted (e.g., `"LP-0001"`).

#### Example Request
```json
{
  "ProcessMethod": "DeleteLPFromWarehouseReceiptLine",
  "Parameters": [
    {
      "LPDocumentNo": "LP-0001"
    }
  ]
}
```

#### Example Response
```json
{
  "Deleted": true,
  "LP_DocumentNo": "LP-0001"
}
```

#### Explanation
- **Deleted**: A boolean value indicating whether the LP was successfully deleted (`true` if deleted, `false` otherwise).
- **LP_DocumentNo**: The document number of the License Plate that was deleted.

#### Process Flow
1. **Validate LP Existence**: The method first checks if the LP exists in the `PLU LP New Headers` table.
2. **Verify LP Status**: It then verifies that the LP is in the "Received" status, which is required for deletion.
3. **Check Warehouse Receipt Association**: The method confirms that the LP is associated with a warehouse receipt line.
4. **Delete LP**: If all checks pass, the LP is deleted from the system.
5. **Return JSON Response**: A JSON response is generated indicating the success of the deletion.

#### Summary
The `DeleteLPFromWarehouseReceiptLine` method provides a secure way to delete License Plates that are associated with warehouse receipt lines. By validating the LP’s existence, status, and association before deletion, this API ensures that only LPs that meet specific criteria are removed. The method returns a JSON response confirming the deletion, which can be used for auditing and tracking purposes.

