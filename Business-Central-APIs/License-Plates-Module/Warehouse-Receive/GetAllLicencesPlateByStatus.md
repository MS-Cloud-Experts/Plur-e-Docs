### API Documentation: GetAllLicencesPlateByStatus

#### Overview
The `GetAllLicencesPlateByStatus` API method retrieves all License Plates (LPs) that match a specified status. This method allows users to filter and retrieve LPs based on their current status in the system.

#### Request Structure
```json
{
  "ProcessMethod": "GetAllLicencesPlateByStatus",
  "Parameters": [
    {
      "LicensePlateStatus": 1
    }
  ]
}
```

#### Parameters
- **LicensePlateStatus**: An integer representing the status of the License Plates to be retrieved. This corresponds to the specific enum value in the system for LP statuses (e.g., `1` for "Received").

#### Example Request
```json
{
  "ProcessMethod": "GetAllLicencesPlateByStatus",
  "Parameters": [
    {
      "LicensePlateStatus": 1
    }
  ]
}
```

#### Example Response
```json
{
  "LicensePlates": [
    {
      "LPDocumentNo": "LP-0001",
      "LocationCode": "LOC01",
      "BinCode": "BIN01",
      "Status": "Received"
    },
    {
      "LPDocumentNo": "LP-0002",
      "LocationCode": "LOC01",
      "BinCode": "BIN02",
      "Status": "Received"
    }
  ]
}
```

#### Explanation
- **LicensePlates**: An array of objects where each object represents a License Plate that matches the specified status.
  - **LPDocumentNo**: The unique identifier for the License Plate (e.g., `"LP-0001"`).
  - **LocationCode**: The code for the location where the License Plate is stored (e.g., `"LOC01"`).
  - **BinCode**: The bin code within the location where the License Plate is stored (e.g., `"BIN01"`).
  - **Status**: The status of the License Plate in human-readable format (e.g., `"Received"`).

#### Summary
The `GetAllLicencesPlateByStatus` method provides a straightforward way to filter and retrieve License Plates based on their current status. This API is useful for warehouse management tasks where tracking the status of LPs is critical. The response includes a list of LPs that meet the specified status criteria, along with relevant location and bin information. This enables users to efficiently manage and monitor the status of LPs within the warehouse system.