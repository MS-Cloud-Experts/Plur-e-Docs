### API Documentation: GetLicencesPlatesByItemNo

#### Overview
The `GetLicencesPlatesByItemNo` API method retrieves detailed information about all License Plates (LPs) that contain a specific item number. The method ensures that each License Plate containing the item is uniquely identified and its full details are returned, including any child LPs associated with it.

#### Request Structure
```json
{
  "ProcessMethod": "GetLicencesPlatesByItemNo",
  "Parameters": [
    {
      "ItemNo": "ITEM001"
    }
  ]
}
```

#### Parameters
- **ItemNo**: The item number for which the License Plates need to be retrieved (e.g., `"ITEM001"`).

#### Example Request
```json
{
  "ProcessMethod": "GetLicencesPlatesByItemNo",
  "Parameters": [
    {
      "ItemNo": "ITEM001"
    }
  ]
}
```

#### Example Response
```json
{
  "LicensePlatesHeaders": [
    {
      "LPDocumentNo": "LP-0001",
      "LicensePlateStatus": "Received",
      "ParentLPNo": "",
      "ZoneCode": "ZONE-01",
      "LocationCode": "LOC01",
      "BinCode": "BIN01",
      "WhseDocumentNo": "WHSE-001",
      "SystemCreatedAt": "2024-08-12T10:00:00",
      "SystemCreatedBy": "UserA",
      "LPTotalQuantities": 100,
      "LPLines": [
        {
          "LineNo": 10000,
          "ItemNo": "ITEM001",
          "VariantCode": "VAR001",
          "SerialNo": "SN001",
          "LotNo": "LOT001",
          "Description": "Item Description 1",
          "Quantity": 50,
          "UnitofMeasure": "PCS"
        }
      ],
      "ChildLPs": [
        {
          "ChildLPDocumentNo": "LP-0001-01",
          "ChildLPStatus": "Stored",
          "ZoneCode": "ZONE-02",
          "LocationCode": "LOC02",
          "BinCode": "BIN02",
          "WhseDocumentNo": "WHSE-002",
          "SystemCreatedAt": "2024-08-12T11:00:00",
          "SystemCreatedBy": "UserB",
          "ChildLPTotalQuantities": 100,
          "LPLines": [
            {
              "LineNo": 20000,
              "ItemNo": "ITEM001",
              "VariantCode": "VAR001",
              "SerialNo": "SN002",
              "LotNo": "LOT002",
              "Description": "Item Description 2",
              "Quantity": 50,
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
- **LicensePlatesHeaders**: An array containing the details of the License Plates that include the specified item number.
  - **LPDocumentNo**: The unique identifier for the License Plate (e.g., `"LP-0001"`).
  - **LicensePlateStatus**: The current status of the License Plate (e.g., `"Received"`).
  - **ParentLPNo**: The document number of the parent LP if this LP is a child, otherwise empty.
  - **ZoneCode**: The code for the zone where the License Plate is stored (e.g., `"ZONE-01"`).
  - **LocationCode**: The code for the location where the License Plate is stored (e.g., `"LOC01"`).
  - **BinCode**: The bin code within the location where the License Plate is stored (e.g., `"BIN01"`).
  - **WhseDocumentNo**: The warehouse document number associated with the License Plate (e.g., `"WHSE-001"`).
  - **SystemCreatedAt**: The timestamp of when the License Plate was created (e.g., `"2024-08-12T10:00:00"`).
  - **SystemCreatedBy**: The user who created the License Plate (e.g., `"UserA"`).
  - **LPTotalQuantities**: The total quantity of items associated with the License Plate.
  - **LPLines**: An array containing the line details of the License Plate.
    - **LineNo**: The line number of the License Plate (e.g., `10000`).
    - **ItemNo**: The item number associated with the line (e.g., `"ITEM001"`).
    - **VariantCode**: The variant code of the item (e.g., `"VAR001"`).
    - **SerialNo**: The serial number of the item (e.g., `"SN001"`).
    - **LotNo**: The lot number of the item (e.g., `"LOT001"`).
    - **Description**: A description of the item (e.g., `"Item Description 1"`).
    - **Quantity**: The quantity of the item in this line (e.g., `50`).
    - **UnitofMeasure**: The unit of measure for the item (e.g., `"PCS"`).
  - **ChildLPs**: An array containing details of any child License Plates associated with this License Plate.
    - **ChildLPDocumentNo**: The unique identifier for the child License Plate (e.g., `"LP-0001-01"`).
    - **ChildLPStatus**: The current status of the child License Plate (e.g., `"Stored"`).
    - **ZoneCode**: The code for the zone where the child License Plate is stored.
    - **LocationCode**: The code for the location where the child License Plate is stored.
    - **BinCode**: The bin code within the location where the child License Plate is stored.
    - **WhseDocumentNo**: The warehouse document number associated with the child License Plate.
    - **SystemCreatedAt**: The timestamp of when the child License Plate was created.
    - **SystemCreatedBy**: The user who created the child License Plate.
    - **ChildLPTotalQuantities**: The total quantity of items associated with the child License Plate.
    - **LPLines**: An array containing the line details of the child License Plate.
    - **ChildLPs**: An array containing any further child License Plates recursively.

#### Summary
The `GetLicencesPlatesByItemNo` API method allows for the retrieval of all License Plates that contain a specific item number, providing full visibility into the storage and tracking of that item across different LPs in the warehouse. The method also includes any associated child LPs, offering a complete view of the item's storage hierarchy.