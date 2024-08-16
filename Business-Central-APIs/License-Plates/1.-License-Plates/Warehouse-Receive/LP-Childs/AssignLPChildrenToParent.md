### API Documentation: AssignLPChildrenToParent

#### Overview
The `AssignLPChildrenToParent` API method assigns a list of child License Plates (LP) to a specified parent LP. This method establishes hierarchical relationships between the specified parent LP and its child LPs in the warehouse management system.

#### Request Structure
```json
{
  "ProcessMethod": "AssignLPChildrenToParent",
  "Parameters": [
    {
      "LPParentDocumentNo": "LP-0001",
      "WarehouseReceipt_No": "WHSE REC-0001",
      "LP_Child": [
        {
          "LP_Child_No": "LP-0002"
        },
        {
          "LP_Child_No": "LP-0003"
        }
      ]
    }
  ]
}
```

#### Parameters
- **LPParentDocumentNo**: The identifier of the parent License Plate (e.g., `"LP-0001"`).
- **WarehouseReceipt_No**: The warehouse receipt number associated with the parent LP (e.g., `"WHSE REC-0001"`).
- **LP_Child**: A JSON array containing objects with the identifiers of the child License Plates to be assigned to the parent LP.

#### Example Request
```json
{
  "ProcessMethod": "AssignLPChildrenToParent",
  "Parameters": [
    {
      "LPParentDocumentNo": "LP-0001",
      "WarehouseReceipt_No": "WHSE REC-0001",
      "LP_Child": [
        {
          "LP_Child_No": "LP-0002"
        },
        {
          "LP_Child_No": "LP-0003"
        }
      ]
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
      "WhseDocumentNo": "WHSE REC-0001",
      "SystemCreatedAt": "2024-08-16T08:45:23Z",
      "SystemCreatedBy": "User1",
      "LPTotalQuantities": 10,
      "LPLines": [
        {
          "LineNo": 10000,
          "ItemNo": "ITEM-001",
          "VariantCode": "VAR-001",
          "SerialNo": "SN-001",
          "LotNo": "LOT-001",
          "Description": "Item Description",
          "Quantity": 10,
          "UnitofMeasure": "PCS"
        }
      ],
      "ChildLPs": [
        {
          "ChildLPDocumentNo": "LP-0002",
          "ChildLPStatus": "Active",
          "ZoneCode": "ZONE1",
          "LocationCode": "LOC1",
          "BinCode": "BIN1",
          "WhseDocumentNo": "WHSE REC-0001",
          "SystemCreatedAt": "2024-08-16T08:45:23Z",
          "SystemCreatedBy": "User1",
          "ChildLPTotalQuantities": 5,
          "LPLines": [
            {
              "LineNo": 10001,
              "ItemNo": "ITEM-002",
              "VariantCode": "VAR-002",
              "SerialNo": "SN-002",
              "LotNo": "LOT-002",
              "Description": "Child Item Description",
              "Quantity": 5,
              "UnitofMeasure": "PCS"
            }
          ],
          "ChildLPs": []
        },
        {
          "ChildLPDocumentNo": "LP-0003",
          "ChildLPStatus": "Active",
          "ZoneCode": "ZONE1",
          "LocationCode": "LOC1",
          "BinCode": "BIN1",
          "WhseDocumentNo": "WHSE REC-0001",
          "SystemCreatedAt": "2024-08-16T08:45:23Z",
          "SystemCreatedBy": "User1",
          "ChildLPTotalQuantities": 8,
          "LPLines": [
            {
              "LineNo": 10002,
              "ItemNo": "ITEM-003",
              "VariantCode": "VAR-003",
              "SerialNo": "SN-003",
              "LotNo": "LOT-003",
              "Description": "Another Child Item",
              "Quantity": 8,
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
- **LicensePlates**: An array of License Plate objects, starting with the parent LP and including all associated child LPs, each with their respective details.
  - **LPDocumentNo**: The document number of the License Plate.
  - **LicensePlateStatus**: The current status of the License Plate.
  - **ParentLPNo**: The document number of the parent LP (if applicable).
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
The `AssignLPChildrenToParent` method is designed to establish parent-child relationships between License Plates in a warehouse setting. By specifying a parent LP and a list of child LPs, this API allows for efficient management of hierarchical inventory structures, which is crucial for accurate tracking and reporting within warehouse operations.
