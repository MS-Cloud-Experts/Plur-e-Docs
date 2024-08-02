### Documentation for the `GetTotalWarehousePickCount` Method

#### Description
The `GetTotalWarehousePickCount` method is used to obtain the total number of warehouse activity lines associated with a specific warehouse shipment number. This method is useful for determining the total number of records available before performing pagination operations.

#### Parameter
- **WarehouseShipmentNo**: `Code[20]`
  - **Description**: The warehouse shipment number for which the total number of activity lines is to be retrieved.
  - **Example**: `'WHSE PICK-02826'`

#### Output
- **Type**: `Integer`
  - **Description**: The total number of warehouse activity lines associated with the provided shipment number.
  - **Example**: `250`

#### Usage
The method is invoked with the warehouse shipment number and returns the total number of associated warehouse activity lines. This is particularly useful for implementing pagination in the user interface or in other methods that require knowledge of the total available records.

#### Example Request
Assume we want to get the total number of warehouse activity lines for the shipment number `'WHSE PICK-02826'`.

**Postman Request:**

- **URL**:`{{baseUrlAPI}}/companies({{CompanyIDMSCE}})/BCApiPlurE({{PageIDMSCE}})/Microsoft.NAV.bcProcessRequest`
- **Method**: `POST`
- **Headers**:
  - `Content-Type: application/json`
- **Body**:
  ```json
  {
    "ProcessMethod": "GetTotalWarehousePickCount",
    "Parameters": [
      {
        "No": "WHSE PICK-02826",
        "WarehouseEmployee": "ASIA1"
      }
    ]
  }
  ```

**Expected Response:**
```json
{
  "TotalCount": 250
}
```

This method can be used in other procedures to determine the total number of records before implementing pagination logic.

### Additional Notes
- This method is particularly useful for applications that require pagination, allowing developers to calculate the total number of pages needed to display all records.

### Conclusion
The `GetTotalWarehousePickCount` method provides an efficient way to count the total number of warehouse activity lines associated with a specific shipment number. This is essential for implementing pagination functionality and improving query performance in the application.