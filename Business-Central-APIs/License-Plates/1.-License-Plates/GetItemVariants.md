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
    }
  ]
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