# API Documentation: PostWarehouseReceipt

## Overview
The `PostWarehouseReceipt` API method processes the posting of a Warehouse Receipt in the system. This method handles validation, execution of the receipt posting, and updates related warehouse activities and employee assignments. It returns information regarding the generated Warehouse Activity and whether the receipt was partially or fully posted.

## Request Structure

```json
{
  "ProcessMethod": "PostWarehouseReceipt",
  "Parameters": [
    {
      "WsheDocumentNo": "WR-0001",
      "WarehouseEmployee": "EMP001"
    }
  ]
}
```

### Parameters

- **No**: The Warehouse Receipt document number to be posted (e.g., `WR-0001`).
- **WarehouseEmployee**: The identifier of the warehouse employee responsible for the receipt (e.g., `EMP001`).

## Example Request

```json
{
  "ProcessMethod": "PostWarehouseReceipt",
  "Parameters": [
    {
      "No": "WR-0001",
      "WarehouseEmployee": "EMP001"
    }
  ]
}
```

## Example Response

```json
{
  "Partial": false,
  "Warehouse_Activity_No": "ACT-0001"
}
```

### Explanation

- **Partial**: Indicates whether the Warehouse Receipt was partially posted. `false` if fully posted.
- **Warehouse_Activity_No**: The identifier of the Warehouse Activity generated during posting.

### Error Handling

If the Warehouse Receipt cannot be posted, the method will return an error message. Example:

```json
{
  "Error": {
    "Code": "Not Posted",
    "Message": "Warehouse Receipt Lines were not found."
  }
}
```

- **Code**: Error code indicating the type of error (e.g., `Not Posted`).
- **Message**: Description of the error (e.g., `Warehouse Receipt Lines were not found.`).

## Summary

The `PostWarehouseReceipt` method is crucial for processing goods receipts into the warehouse. It performs necessary validations, correctly posts the receipt, and updates relevant warehouse activities. The method provides information about the Warehouse Activity associated with the receipt, allowing further tracking and processing. Detailed error information is provided if any issues occur during posting.
