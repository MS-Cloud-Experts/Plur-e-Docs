### API Documentation: `GetBinContentByItemLocation`

#### Overview
The `GetBinContentByItemLocation` API retrieves detailed information about the contents of a specific bin within a given location for a specified item and unit of measure. It returns total quantities along with a breakdown of quantities in each License Plate (LP) associated with that item.

#### Request Structure
```json
{
  "ProcessMethod": "GetBinContentByItemLocation",
  "Parameters": [
    {
      "ItemNo": "D0AVESVTBLU00S",
      "VariantCode": "",
      "LocationCode": "MAIN",
      "BinCode": "10A1",
      "UnitofMeasureCode": "EA"
    }
  ]
}
```

#### Parameters
- **BinCode**: The code of the bin where the item is stored (e.g., `"STO1"`).
- **LocationCode**: The location where the bin is situated (e.g., `"CCC"`).
- **ItemNo**: The identifier for the item to retrieve from the bin (e.g., `"1900-S"`).
- **UnitofMeasureCode**: The unit of measure used for the item (e.g., `"PCS"`).

#### Example Request
```json
{
  "ProcessMethod": "GetBinContentByItemLocation",
  "Parameters": [
    {
      "ItemNo": "D0AVESVTBLU00S",
      "VariantCode": "",
      "LocationCode": "MAIN",
      "BinCode": "BACK",
      "UnitofMeasureCode": "EA"
    }
  ]
}
```

#### Example Response
```json
{
  "ItemNo": "D1BDBKCBBLASTD",
  "VariantCode": "",
  "UnitofMeasureCode": "EA",
  "LocationCode": "MAIN",
  "BinCode": "10A1",
  "TotalQtyAvailToTakeUOM": 235.0,
  "TotalQtyAvailToPick": 235.0,
  "TotalQtyAvailToPutAway": -235.0,
  "TotalQtyInBinContent": 235.0,
  "TotalQtyToTake": 235.0,
  "TotalQtyInLP": 214.0,
  "Details": [
    {
      "LP": "LP-00011",
      "Qty": "5"
    },
    {
      "LP": "LP-00011",
      "Qty": "10"
    },
    {
      "LP": "LP-00011",
      "Qty": "5"
    },
    {
      "LP": "LP-00013",
      "Qty": "5"
    },
    {
      "LP": "LP-00014",
      "Qty": "5"
    },
    {
      "LP": "LP-00015",
      "Qty": "5"
    },
    {
      "LP": "LP-00016",
      "Qty": "5"
    },
    {
      "LP": "LP-00028",
      "Qty": "4"
    },
    {
      "LP": "LP-00028",
      "Qty": "3"
    },
    {
      "LP": "LP-00039",
      "Qty": "3"
    },
    {
      "LP": "LP-00052",
      "Qty": "2"
    },
    {
      "LP": "LP-00052",
      "Qty": "10"
    },
    {
      "LP": "LP-00052",
      "Qty": "6"
    },
    {
      "LP": "LP-00052",
      "Qty": "10"
    },
    {
      "LP": "LP-00052",
      "Qty": "5"
    },
    {
      "LP": "LP-00052",
      "Qty": "10"
    },
    {
      "LP": "LP-00052",
      "Qty": "3"
    },
    {
      "LP": "LP-00052",
      "Qty": "3"
    },
    {
      "LP": "LP-00053",
      "Qty": "5"
    },
    {
      "LP": "LP-00062",
      "Qty": "10"
    },
    {
      "LP": "LP-00063",
      "Qty": "3"
    },
    {
      "LP": "LP-00066",
      "Qty": "1"
    },
    {
      "LP": "LP-00067",
      "Qty": "2"
    },
    {
      "LP": "LP-00070",
      "Qty": "20"
    },
    {
      "LP": "LP-00072",
      "Qty": "2"
    },
    {
      "LP": "LP-00074",
      "Qty": "4"
    },
    {
      "LP": "LP-00076",
      "Qty": "1"
    },
    {
      "LP": "LP-00079",
      "Qty": "3"
    },
    {
      "LP": "LP-00079",
      "Qty": "4"
    },
    {
      "LP": "LP-00081",
      "Qty": "3"
    },
    {
      "LP": "LP-00081",
      "Qty": "1"
    },
    {
      "LP": "LP-00081",
      "Qty": "1"
    },
    {
      "LP": "LP-00084",
      "Qty": "5"
    },
    {
      "LP": "LP-00084",
      "Qty": "6"
    },
    {
      "LP": "LP-00084",
      "Qty": "4"
    },
    {
      "LP": "LP-00084",
      "Qty": "10"
    },
    {
      "LP": "LP-00084",
      "Qty": "5"
    },
    {
      "LP": "LP-00084",
      "Qty": "15"
    },
    {
      "LP": "LP-00084",
      "Qty": "10"
    }
  ],
  "Duration": "44 milliseconds"
}
```

#### Response Fields
- **TotalQty**: The total quantity of the item available in the bin.
- **TotalQtyInLP**: The total quantity of the item calculated from the License Plates in the bin.
- **Details**: An array containing details of each License Plate (LP) in the bin.
  - **LP**: The License Plate identifier.
  - **Qty**: The quantity of the item associated with the LP.

#### Explanation
- **TotalQty**: The cumulative quantity of the specified item in the bin.
- **TotalQtyInLP**: The total quantity calculated from the LPs containing the item in the bin.
- **Details**: A breakdown of each License Plate (LP) storing the item and the quantity in each LP.

#### Process Flow
1. **Parse Input**: The API takes in `LocationCode`, `BinCode`, `ItemNo`, and `UnitofMeasureCode` as input parameters.
2. **Fetch Bin Content**: It retrieves movements of the specified item within the location and bin, filtered by the item number and unit of measure.
3. **Calculate Quantities**: It calculates the total quantity of the item in the bin and breaks down quantities by each LP.
4. **Return Response**: The API responds with the total quantities and a detailed list of LPs and their associated quantities.

#### Example Use Case
If a warehouse manager wants to know the contents of bin "STO1" in location "CCC" for item "1900-S" (measured in PCS), this API will return the total quantity of the item and a detailed list of License Plates (LPs) in that bin, along with how much of the item is stored in each LP.

#### Summary
The `GetBinContentByItemLocation` API is an essential tool for warehouse operations, providing detailed information about the contents of a specific bin for a particular item. It ensures that all License Plates storing the item are accurately accounted for, facilitating efficient warehouse management and stock control.