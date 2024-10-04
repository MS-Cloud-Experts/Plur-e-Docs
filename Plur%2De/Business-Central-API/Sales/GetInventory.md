### API Documentation: GetInventory

#### Overview
The `GetInventory` API method retrieves detailed information about inventory items based on various parameters such as Item Number, Variant Code, Serial Number, Unit of Measure, and Location Code. It allows users to specify multiple parameters to obtain relevant inventory data, including available quantities by different variants and units of measure.

#### Request Structure
```json
{
  "ProcessMethod": "GetInventory",
  "Parameters": [
    {
      "ItemNo": "SERIAL",
      "VariantCode": "",
      "SerialNo": "",
      "UnitofMeasureCode": "PCS",
      "LocationCode": "FTLDL-RET"
    }
  ]
}
```

#### Parameters
- **ItemNo**: The unique identifier for the item to be retrieved (e.g., `"ITEM001"`). This parameter is optional, but if not provided, the inventory will be retrieved based on other criteria such as serial number.
- **VariantCode**: The variant code of the item, if applicable (e.g., `"VAR001"`).
- **SerialNo**: The serial number of the item, if applicable (e.g., `"SN001"`).
- **UnitofMeasureCode**: The unit of measure for the item (e.g., `"PCS"`).
- **LocationCode**: The code for the location from which inventory data should be retrieved (e.g., `"LOC01"`).

#### Example Request
```json
{
  "ProcessMethod": "GetInventory",
  "Parameters": [
    {
      "ItemNo": "SERIAL",
      "VariantCode": "",
      "SerialNo": "",
      "UnitofMeasureCode": "PCS",
      "LocationCode": "FTLDL-RET"
    }
  ]
}
```

#### Example Response
```json
{
  "Inventory": [
    {
      "ItemNo": "SERIAL",
      "VariantCode": "",
      "LocationCode": "FTLDL-RET",
      "ItemQty": [
        {
          "ItemNo": "SERIAL",
          "VariantCode": "",
          "UnitofMeasureCode": "EA",
          "Quantity": 3.0,
          "SerialArray": [
            {
              "ItemNo": "SERIAL",
              "VariantCode": "",
              "LocationCode": "FTLDL-RET",
              "SerialNo": "X1",
              "Quantity": 1.0
            },
            {
              "ItemNo": "SERIAL",
              "VariantCode": "",
              "LocationCode": "FTLDL-RET",
              "SerialNo": "X2",
              "Quantity": 1.0
            },
            {
              "ItemNo": "SERIAL",
              "VariantCode": "",
              "LocationCode": "FTLDL-RET",
              "SerialNo": "X3",
              "Quantity": 1.0
            }
          ],
          "LotArray": []
        }
      ],
      "QtyXVariants": []
    }
  ],
  "Duration": "4 seconds 639 milliseconds"
}
```

#### Explanation
- **Inventory**: An array containing the details of the requested inventory items.
  - **ItemNo**: The unique identifier for the item (e.g., `"ITEM001"`).
  - **VariantCode**: The variant code of the item (e.g., `"VAR001"`).
  - **LocationCode**: The code for the location where the item is stored (e.g., `"LOC01"`).
  - **ItemQty**: An array providing quantities of the item by different units of measure.
    - **UnitofMeasureCode**: The unit of measure for the item (e.g., `"PCS"`).
    - **Quantity**: The available quantity for the specified unit of measure (e.g., `100`).
  - **QtyXVariants**: An array providing quantities by different variants.
    - **VariantCode**: The variant code of the item (e.g., `"VAR001"`).
    - **UnitofMeasureCode**: The unit of measure for the variant (e.g., `"PCS"`).
    - **Quantity**: The available quantity for the specified variant (e.g., `100`).

#### Summary
The `GetInventory` API method provides comprehensive inventory information based on various parameters, including Item Number, Variant Code, Serial Number, Location Code, and Unit of Measure. This flexibility allows users to obtain accurate and relevant inventory details, including total quantities by unit of measure and variant. The detailed response ensures users can effectively manage inventory and gain visibility into the availability of specific items in the warehouse.

