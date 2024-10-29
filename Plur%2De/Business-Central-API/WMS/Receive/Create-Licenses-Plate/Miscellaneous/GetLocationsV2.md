### API Documentation: GetLocationsV2

#### Overview
The `GetLocationsV2` API method provides a list of warehouse locations associated with a specified company. This method enables efficient retrieval of location details, including location codes, names, and various warehouse handling parameters, supporting inventory and logistics management.

#### Request Structure
```json
{
  "ProcessMethod": "GetLocationsV2",
  "Parameters": [
    {
      "CompanyName": "Adventure Sports USA"
    }
  ]
}
```

#### Parameters
- **CompanyName**: The name of the company whose locations are to be retrieved (e.g., `"Adventure Sports USA"`).

#### Example Request
```json
{
  "ProcessMethod": "GetLocationsV2",
  "Parameters": [
    {
      "CompanyName": "Adventure Sports USA"
    }
  ]
}
```

#### Example Response
```json
{
  "Location": [
    {
      "Code": "ASIA",
      "Name": "ASIA - CABRINHA WAREHOUSE",
      "DirectedPutAwayandPick": false,
      "Allow Line Reuse": false,
      "AllowRegisterPick": false,
      "CompanyName": "Adventure Sports USA"
    },
    {
      "Code": "MAIN",
      "Name": "MAIN WAREHOUSE",
      "DirectedPutAwayandPick": true,
      "Allow Line Reuse": true,
      "AllowRegisterPick": true,
      "CompanyName": "Adventure Sports USA"
    }
    // Additional locations omitted for brevity
  ]
}
```

#### Explanation
- **Location**: An array of location objects containing details of each warehouse location. Each object includes:
  - **Code**: The unique identifier for the location (e.g., `"ASIA"`).
  - **Name**: The name of the location (e.g., `"ASIA - CABRINHA WAREHOUSE"`).
  - **DirectedPutAwayandPick**: Boolean indicating if directed put-away and pick is enabled for this location.
  - **Allow Line Reuse**: Boolean indicating if line reuse is allowed within the location.
  - **AllowRegisterPick**: Boolean indicating if pick registrations are permitted at the location.
  - **CompanyName**: The company to which the location belongs.

#### Summary
The `GetLocationsV2` API provides a structured way to retrieve detailed information on warehouse locations within a specific company. It enables users to access relevant location attributes like handling and operational settings, which assist in managing inventory distribution effectively. This method is essential for warehouse and logistics operations, as it allows precise control over inventory management settings across various storage locations, enhancing operational flexibility and traceability.