## **API Documentation: CreateEmptyLPFromWarehouseReceipt**

### **Overview**
The `CreateEmptyLPFromWarehouseReceipt` API method allows for the creation of an empty License Plate (LP) associated with a specific Warehouse Receipt. This method is useful when you need to generate an LP header without any line items, linking it directly to an existing Warehouse Receipt document.

### **Request Structure**

```json
{
  "ProcessMethod": "CreateEmptyLPFromWarehouseReceipt",
  "Parameters": [
    {
      "WarehouseReceiptNo": "WR-0001"
    }
  ]
}
```

#### **Parameters**
- **WarehouseReceiptNo**: The document number of the Warehouse Receipt with which the new LP will be associated (e.g., `"WR-0001"`).

### **Example Request**

```json
{
  "ProcessMethod": "CreateEmptyLPFromWarehouseReceipt",
  "Parameters": [
    {
      "WarehouseReceiptNo": "WR-0001"
    }
  ]
}
```

### **Example Response**

```json
{
  "LPDocumentNo": "LP-0001"
}
```

#### **Explanation**

- **LPDocumentNo**: The document number of the newly created License Plate (e.g., `"LP-0001"`).

### **Process Description**

1. **Parse Parameters:**
   - The method parses the input parameters to retrieve the `WarehouseReceiptNo`.

2. **Validate Warehouse Receipt:**
   - The system checks if the Warehouse Receipt exists using the `WarehouseReceiptNo`. If it does not exist, an error message is generated.

3. **Create Empty License Plate:**
   - The method calls `Create_Manual_LP_From_WarehouseReceipt`, which generates a new License Plate associated with the specified Warehouse Receipt. Only the LP header is created, without any line items.

4. **Return JSON Response:**
   - The method returns a JSON object containing the `LPDocumentNo`, which confirms the successful creation of the License Plate.

### **Error Handling**
- If the specified Warehouse Receipt does not exist, the system will return an error message indicating the issue.

### **Summary**
The `CreateEmptyLPFromWarehouseReceipt` method is designed for scenarios where an LP header needs to be generated and associated with an existing Warehouse Receipt document. This operation ensures that the LP is correctly linked to the Warehouse Receipt, facilitating further inventory management processes.

