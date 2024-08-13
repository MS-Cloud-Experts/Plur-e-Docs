### API Documentation: Post_WarehousePutAway

#### Overview
The `Post_WarehousePutAway` API method is used to process and post Warehouse Put-Away activities. This method registers the put-away operations in the warehouse, ensuring that inventory is correctly moved and recorded in the system.

#### Request Structure
```json
{
  "ProcessMethod": "Post_WarehousePutAway",
  "Parameters": [
    {
      "WsheDocumentNo": "PA-0001",
      "WarehouseEmployee": "EMP001"
    }
  ]
}
```

#### Parameters
- **WsheDocumentNo**: The Warehouse Activity document number that identifies the put-away operation to be posted (e.g., `"PA-0001"`).

#### Example Request
```json
{
  "ProcessMethod": "Post_WarehousePutAways",
  "Parameters": [
    {
      "WsheDocumentNo": "PA-0001"
    }
  ]
}
```

#### Example Response
```json
{
  "Registered_Whse_Activity": "REG-0001"
}
```

#### Explanation
- **Registered_Whse_Activity**: The number of the registered warehouse activity document created after the successful posting of the put-away operation (e.g., `"REG-0001"`).

#### Summary
The `Post_WarehousePutAways` method is integral to the warehouse management process as it automates the posting of put-away operations. By using this API, the system registers the movement of inventory from receiving bins to storage bins, ensuring that the warehouse records are up to date and accurate. The method returns the registered warehouse activity number, which can be used for further tracking and audit purposes.

This documentation provides a detailed overview of the API, including the request structure, parameters, and example responses, to assist developers in integrating and utilizing this functionality effectively.
