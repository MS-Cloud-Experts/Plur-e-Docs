### API Documentation: GetItemVariants

#### Overview
The `GetItemVariants` API retrieves all items along with their respective variants from the system. The result includes key information such as item numbers, descriptions, base units of measure, and tracking codes. Additionally, it provides detailed information on the variants associated with each item.

#### Request Structure
There are no parameters required for this API.

#### Example Request
```json
{
  "ProcessMethod": "GetItemVariants",
  "Parameters": []
}
```

#### Response Structure
The API returns a list of items with the following structure:

```json
{
  "Items": [
    {
      "No": "ITEM001",
      "Description": "Sample Item 1",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [
        {
          "ItemNo": "ITEM001",
          "VariantCode": "V001",
          "Description": "Variant 1"
        },
        {
          "ItemNo": "ITEM001",
          "VariantCode": "V002",
          "Description": "Variant 2"
        }
      ],
      "ManagedbyPlurE": true,
      "ItemTrackingCode": "SNTRACK",
      "SN Warehouse Tracking": true,
      "Lot Warehouse Tracking": false
    },
    {
      "No": "ITEM002",
      "Description": "Sample Item 2",
      "BaseUnitofMeasure": "BOX",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": "LOTTRACK",
      "SN Warehouse Tracking": false,
      "Lot Warehouse Tracking": true
    }
  ]
}
```

#### Parameters
No input parameters are required for this API. It retrieves all available items and their variants.

#### Response Fields
- **Items**: An array containing all items retrieved from the system.
  - **No**: The item number.
  - **Description**: The description of the item.
  - **BaseUnitofMeasure**: The base unit of measure for the item.
  - **VariantArray**: An array containing the variants associated with the item.
    - **ItemNo**: The item number of the variant.
    - **VariantCode**: The variant code.
    - **Description**: The description of the variant.
  - **ManagedbyPlurE**: A boolean value indicating if the item is managed by Plur-E.
  - **ItemTrackingCode**: The tracking code associated with the item.
  - **SN Warehouse Tracking**: A boolean indicating if serial number tracking is enabled in the warehouse.
  - **Lot Warehouse Tracking**: A boolean indicating if lot tracking is enabled in the warehouse.

#### Example Response
```json
{
  "Items": [
    {
      "No": "1005",
      "Description": "1005.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": "LOTALL",
      "SN Warehouse Tracking": false,
      "Lot Warehouse Tracking": true
    },
    {
      "No": "1006",
      "Description": "1006.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": true,
      "ItemTrackingCode": "SNALL",
      "SN Warehouse Tracking": true,
      "Lot Warehouse Tracking": false
    },
    {
      "No": "1007",
      "Description": "SERIAL.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": "SNALL",
      "SN Warehouse Tracking": true,
      "Lot Warehouse Tracking": false
    },
    {
      "No": "1008",
      "Description": "SERIAL2.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": "SNALL",
      "SN Warehouse Tracking": true,
      "Lot Warehouse Tracking": false
    },
    {
      "No": "1009",
      "Description": "1009.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1010",
      "Description": "managed by plure.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": true,
      "ItemTrackingCode": ""
    },
    {
      "No": "1012",
      "Description": "",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1013",
      "Description": "managed by plure with serial",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": true,
      "ItemTrackingCode": "SNALL",
      "SN Warehouse Tracking": true,
      "Lot Warehouse Tracking": false
    },
    {
      "No": "1014",
      "Description": "managed by plure with serial",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": true,
      "ItemTrackingCode": "SNALL",
      "SN Warehouse Tracking": true,
      "Lot Warehouse Tracking": false
    },
    {
      "No": "1896-S",
      "Description": "ATHENS Desk.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [
        {
          "ItemNo": "1896-S",
          "VariantCode": "001",
          "Description": "001"
        },
        {
          "ItemNo": "1896-S",
          "VariantCode": "002",
          "Description": "002"
        },
        {
          "ItemNo": "1896-S",
          "VariantCode": "003",
          "Description": "003"
        }
      ],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1900-S",
      "Description": "PARIS Guest Chair, black.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1906-S",
      "Description": "ATHENS Mobile Pedestal.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1908-S",
      "Description": "LONDON Swivel Chair, blue.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1920-S",
      "Description": "ANTWERP Conference Table.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1925-W",
      "Description": "Conference Bundle 1-6.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1928-S",
      "Description": "AMSTERDAM Lamp.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1929-W",
      "Description": "Conference Bundle 1-8.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1936-S",
      "Description": "BERLIN Guest Chair, yellow.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1953-W",
      "Description": "Guest Section 1.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1960-S",
      "Description": "ROME Guest Chair, green.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1964-S",
      "Description": "TOKYO Guest Chair, blue.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1965-W",
      "Description": "Conference Bundle 2-8.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1968-S",
      "Description": "MEXICO Swivel Chair, black.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1969-W",
      "Description": "Conference Package 1.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1972-S",
      "Description": "MUNICH Swivel Chair, yellow.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1980-S",
      "Description": "MOSCOW Swivel Chair, red.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1988-S",
      "Description": "SEOUL Guest Chair, red.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "1996-S",
      "Description": "ATLANTA Whiteboard, base.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "2000-S",
      "Description": "SYDNEY Swivel Chair, green.",
      "BaseUnitofMeasure": "PCS",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    },
    {
      "No": "MY FIRST ITEM",
      "Description": "Description Modifyed.",
      "BaseUnitofMeasure": "",
      "VariantArray": [],
      "ManagedbyPlurE": false,
      "ItemTrackingCode": ""
    }
  ],
  "Duration": "285 milliseconds"
}
```

#### Process Flow
1. **Retrieve Items**: The system fetches all items from the `Item` table.
2. **Fetch Variants**: For each item, the system checks the `Item Variant` table to retrieve all associated variants.
3. **Tracking Code Information**: The system checks the `Item Tracking Code` table for each item to retrieve the serial number and lot tracking settings.
4. **Return Response**: The system formats the data into a JSON object and returns the list of items and their variants.

#### Considerations
- **Data Integrity**: Ensure that all items have valid tracking codes and that variants are properly associated with the correct item.
- **Empty Variants**: If an item does not have variants, the `VariantArray` field will be returned as an empty array.

#### Summary
The `GetItemVariants` API is designed to provide a comprehensive overview of items and their variants, including item tracking information. This method is useful for systems that need to track item variants and ensure accurate warehouse and inventory management.