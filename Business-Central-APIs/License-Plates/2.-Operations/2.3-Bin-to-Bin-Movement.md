### API Documentation: MoveBinToBinLP

#### Overview
The `MoveBinToBinLP` API method facilitates the movement of License Plates (LPs) from one bin to another within a warehouse. This process updates the system's records to reflect the new bin locations for the LPs, ensuring accurate inventory tracking.

#### Request Structure
```json
{
  "ProcessMethod": "MoveBinToBinLP",
  "Parameters": [
    {
      "LPToMove": [
        {
          "LPDocumentNo": "LP001",
          "FromBin": "BIN-01",
          "ToBin": "BIN-02"
        },
        {
          "LPDocumentNo": "LP002",
          "FromBin": "BIN-01",
          "ToBin": "BIN-03"
        }
      ]
    }
  ]
}
```

#### Parameters
- **ProcessMethod**: Indicates the method to be invoked, in this case, `"MoveBinToBinLP"`.
- **Parameters**: A JSON array containing the list of LPs to be moved.
  - **LPToMove**: An array of objects, each representing an LP to be moved.
    - **LPDocumentNo**: The document number of the LP to be moved (e.g., `"LP001"`).
    - **FromBin**: The current bin code from which the LP is being moved (e.g., `"BIN-01"`).
    - **ToBin**: The target bin code to which the LP is being moved (e.g., `"BIN-02"`).

#### Example Request
```json
{
  "ProcessMethod": "MoveBinToBinLP",
  "Parameters": [
    {
      "LPToMove": [
        {
          "LPDocumentNo": "LP001",
          "FromBin": "BIN-01",
          "ToBin": "BIN-02"
        },
        {
          "LPDocumentNo": "LP002",
          "FromBin": "BIN-01",
          "ToBin": "BIN-03"
        }
      ]
    }
  ]
}
```

#### Example Response
```json
{
  "Message": "The LPs were moved successfully.",
  "MovedLPs": [
    {
      "LPDocumentNo": "LP001",
      "FromBin": "BIN-01",
      "ToBin": "BIN-02"
    },
    {
      "LPDocumentNo": "LP002",
      "FromBin": "BIN-01",
      "ToBin": "BIN-03"
    }
  ]
}
```

#### Explanation
- **Message**: A confirmation message indicating that the LPs were moved successfully.
- **MovedLPs**: A list of LPs that were moved, showing their document numbers, original bins, and new bins.

#### Summary
The `MoveBinToBinLP` method automates the process of relocating License Plates (LPs) from one bin to another within a warehouse. By validating the input data and performing the necessary updates, this API ensures that LPs are accurately tracked as they are moved to new locations. The method returns a detailed confirmation of the LPs that were successfully moved, which is crucial for maintaining accurate inventory records.