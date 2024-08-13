### API Documentation: GetItemInfo

#### Overview
The `GetItemInfo` API method retrieves detailed information about a specific item within the warehouse system. This method checks if the item is managed by the Plur-E system and whether it has automatic generation settings for serial numbers (SN) and lot numbers (LOT).

#### Request Structure
```json
{
  "ProcessMethod": "GetItemInfo",
  "Parameters": [
    {
      "ItemNo": "1900-S"
    }
  ]
}
```

#### Parameters
- **ItemNo**: The unique identifier for the item for which information is being requested (e.g., `"1900-S"`).

#### Example Request
```json
{
  "ProcessMethod": "GetItemInfo",
  "Parameters": [
    {
      "ItemNo": "1900-S"
    }
  ]
}
```

#### Example Response
```json
{
  "ItemNo": "1900-S",
  "Managed_by_PlurE": true,
  "Auto_Generate_SN": false,
  "Auto_Generate_LOT": false
}
```

#### Explanation
- **ItemNo**: The item number that was queried (e.g., `"1900-S"`).
- **Managed_by_PlurE**: Indicates whether the item is managed by the Plur-E system (`true` or `false`).
- **Auto_Generate_SN**: Specifies whether the system automatically generates serial numbers for this item (`true` or `false`).
- **Auto_Generate_LOT**: Specifies whether the system automatically generates lot numbers for this item (`true` or `false`).

#### Summary
The `GetItemInfo` method provides essential details about an item, focusing on its management by the Plur-E system and its automatic number generation settings. This information is crucial for ensuring that items are correctly tracked and managed within the warehouse system. The method returns the item number along with its management and generation settings, aiding in inventory control and accuracy.