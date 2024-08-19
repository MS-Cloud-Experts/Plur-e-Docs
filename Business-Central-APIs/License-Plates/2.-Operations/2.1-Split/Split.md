### API Documentation: SplitLP

#### Overview
The `SplitLP` API method facilitates the splitting of an existing License Plate (LP) into multiple new LPs based on specified quantities for each line within the LP. This method validates the input data, processes each line to be split, creates new LPs, and registers the corresponding movements.

#### Request Structure
```json
{
  "ProcessMethod": "SplitLP",
  "Parameters": [
    {
      "LPDocumentNo": "LP001",
      "LinesToSplit": [
        {
          "LPLineNo": 1000,
          "QuantityToSplit": 60
        },
        {
          "LPLineNo": 2000,
          "QuantityToSplit": 40
        }
      ]
    }
  ]
}
```

#### Parameters
- **LPDocumentNo**: The document number of the License Plate (LP) to be split (e.g., `"LP001"`).
- **LinesToSplit**: An array of objects specifying the lines within the LP that need to be split. Each object should contain:
  - **LPLineNo**: The line number within the LP that is being split (e.g., `1000`).
  - **QuantityToSplit**: The quantity from the line that should be split into a new LP (e.g., `60`).

#### Example Request
```json
{
  "ProcessMethod": "SplitLP",
  "Parameters": [
    {
      "LPDocumentNo": "LP001",
      "LinesToSplit": [
        {
          "LPLineNo": 1000,
          "QuantityToSplit": 60
        },
        {
          "LPLineNo": 2000,
          "QuantityToSplit": 40
        }
      ]
    }
  ]
}
```

#### Example Response
```json
{
  "OriginalLP": "LP001",
  "NewLPs": [
    {
      "LPDocumentNo": "LP002",
      "CreatedFromLineNo": 1000,
      "Quantity": 60
    },
    {
      "LPDocumentNo": "LP003",
      "CreatedFromLineNo": 2000,
      "Quantity": 40
    }
  ],
  "Message": "The LP has been successfully split."
}
```

#### Explanation
- **OriginalLP**: The original License Plate document number that was split.
- **NewLPs**: An array of objects detailing the new LPs created during the split. Each object contains:
  - **LPDocumentNo**: The document number of the new LP created.
  - **CreatedFromLineNo**: The line number from the original LP that was split to create this new LP.
  - **Quantity**: The quantity assigned to the new LP.
- **Message**: A message indicating the outcome of the operation.

#### Summary
The `SplitLP` method is designed to automate the process of splitting a License Plate (LP) into multiple new LPs. This method allows for flexible handling of inventory by splitting specific quantities from selected lines within the original LP. The method ensures that the original LP is only destroyed if all quantities have been reallocated, maintaining data integrity and providing detailed tracking of the newly created LPs.

This API method is essential for warehouse operations where managing and splitting inventory efficiently is crucial, providing a seamless way to handle LPs and their contents across various storage bins and locations.