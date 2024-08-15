### API Documentation: GetLicencesPlateByWsheDocument

#### Overview
The `GetLicencesPlateByWsheDocument` API method retrieves all License Plates (LPs) associated with a specific warehouse document. This method provides detailed information about each LP found, including any child LPs that are related to the specified warehouse document.

#### Request Structure
```json
{
  "ProcessMethod": "GetLicencesPlateByWsheDocument",
  "Parameters": [
    {
      "WsheDocumentNo": "WHSE DOC-0001"
    }
  ]
}
```

#### Parameters
- **WsheDocumentNo**: The warehouse document number for which the associated License Plates should be retrieved (e.g., `"WHSE DOC-0001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetLicencesPlateByWsheDocument",
  "Parameters": [
    {
       "WsheDocumentNo": "WHSE DOC-0001"
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
      "LicensePlateStatus": "Active",
      "ParentLPNo": "",
      "ZoneCode": "ZONE1",
      "LocationCode": "LOC1",
      "BinCode": "BIN1",
      "WhseDocumentNo": "WHSE DOC-0001",
      "SystemCreatedAt": "2024-08-16T08:45:23Z",
      "SystemCreatedBy": "User1",
      "LPTotalQuantities": 100,
      "LPLines": [
        {
          "LineNo": 10000,
          "ItemNo": "ITEM-001",
          "VariantCode": "VAR-001",
          "SerialNo": "SN-001",
          "LotNo": "LOT-001",
          "Description": "Item Description",
          "Quantity": 100,
          "UnitofMeasure": "PCS"
        }
      ],
      "ChildLPs": []
    },
    {
      "LPDocumentNo": "LP-0002",
      "LicensePlateStatus": "Active",
      "ParentLPNo": "LP-0001",
      "ZoneCode": "ZONE2",
      "LocationCode": "LOC2",
      "BinCode": "BIN2",
      "WhseDocumentNo": "WHSE DOC-0001",
      "SystemCreatedAt": "2024-08-16T09:12:47Z",
      "SystemCreatedBy": "User2",
      "LPTotalQuantities": 50,
      "LPLines": [
        {
          "LineNo": 10001,
          "ItemNo": "ITEM-002",
          "VariantCode": "VAR-002",
          "SerialNo": "SN-002",
          "LotNo": "LOT-002",
          "Description": "Another Item Description",
          "Quantity": 50,
          "UnitofMeasure": "PCS"
        }
      ],
      "ChildLPs": [
        {
          "ChildLPDocumentNo": "LP-0003",
          "ChildLPStatus": "Active",
          "ZoneCode": "ZONE2",
          "LocationCode": "LOC2",
          "BinCode": "BIN2",
          "WhseDocumentNo": "WHSE DOC-0001",
          "SystemCreatedAt": "2024-08-16T09:30:10Z",
          "SystemCreatedBy": "User3",
          "ChildLPTotalQuantities": 25,
          "LPLines": [
            {
              "LineNo": 10002,
              "ItemNo": "ITEM-003",
              "VariantCode": "VAR-003",
              "SerialNo": "SN-003",
              "LotNo": "LOT-003",
              "Description": "Child Item Description",
              "Quantity": 25,
              "UnitofMeasure": "PCS"
            }
          ],
          "ChildLPs": []
        }
      ]
    }
  ]
}
```

#### Explanation
- **LicensePlates**: An array of License Plate objects associated with the specified warehouse document.
  - **LPDocumentNo**: The document number of the License Plate.
  - **LicensePlateStatus**: The current status of the License Plate.
  - **ParentLPNo**: The document number of the parent LP, if applicable.
  - **ZoneCode**: The zone code where the LP is stored.
  - **LocationCode**: The location code of the LP.
  - **BinCode**: The bin code of the LP.
  - **WhseDocumentNo**: The associated warehouse document number.
  - **SystemCreatedAt**: Timestamp when the LP was created.
  - **SystemCreatedBy**: User who created the LP.
  - **LPTotalQuantities**: Total quantities of items in the LP.
  - **LPLines**: An array of item lines associated with the LP, each containing:
    - **LineNo**: The line number.
    - **ItemNo**: The item number.
    - **VariantCode**: The variant code of the item.
    - **SerialNo**: The serial number of the item.
    - **LotNo**: The lot number of the item.
    - **Description**: The description of the item.
    - **Quantity**: The quantity of the item.
    - **UnitofMeasure**: The unit of measure of the item.
  - **ChildLPs**: Recursively lists child LPs associated with this LP, following the same structure.

#### Summary
The `GetLicencesPlateByWsheDocument` method is designed to retrieve all License Plates associated with a specific warehouse document. This API is essential for tracking and managing License Plates within a warehouse environment, providing detailed information on each LP, including any hierarchical relationships between parent and child LPs.

