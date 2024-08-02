## API Documentation: GetPagedWarehousePick

### Overview
The `GetPagedWarehousePick` API method allows for paginated retrieval of warehouse pick lines. This enables efficient handling of large datasets by fetching a limited number of lines per request.

### Request Structure
```json
{
  "ProcessMethod": "GetPagedWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-02826",
      "WarehouseEmployee": "ASIA1",
      "Limit": 2,
      "Offset": 2
    }
  ]
}
```

### Parameters
- **No**: The warehouse pick number (e.g., "WHSE PICK-02826").
- **WarehouseEmployee**: The identifier for the warehouse employee (e.g., "ASIA1").
- **Limit**: The number of lines to retrieve per request (e.g., 2).
- **Offset**: The starting point for the lines to retrieve, beginning at 1 (e.g., 2).

### Example Requests and Responses
#### First Request: Offset = 1
**Request:**
```json
{
  "ProcessMethod": "GetPagedWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-02826",
      "WarehouseEmployee": "ASIA1",
      "Limit": 2,
      "Offset": 1
    }
  ]
}
```
**Response:**
```json
{
  "Lines": [
    {
      "LineNo": 10000,
      "ItemNo": "K2CSODQLC",
      "VariantCode": "LRGXXX",
      "BinCode": "STORAGE"
    },
    {
      "LineNo": 20000,
      "ItemNo": "K2CSODQLC",
      "VariantCode": "LRGXXX",
      "BinCode": "SHIP"
    }
  ]
}
```

#### Second Request: Offset = 2
**Request:**
```json
{
  "ProcessMethod": "GetPagedWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-02826",
      "WarehouseEmployee": "ASIA1",
      "Limit": 2,
      "Offset": 2
    }
  ]
}
```
**Response:**
```json
{
  "Lines": [
    {
      "LineNo": 30000,
      "ItemNo": "K2CSODQLC",
      "VariantCode": "LRGXXX",
      "BinCode": "STORAGE"
    },
    {
      "LineNo": 40000,
      "ItemNo": "K2CSODQLC",
      "VariantCode": "LRGXXX",
      "BinCode": "SHIP"
    }
  ]
}
```

### Explanation
- **First Request (Offset = 1)**: Retrieves the first two lines (LineNo 10000 and 20000).
- **Second Request (Offset = 2)**: Retrieves the next two lines (LineNo 30000 and 40000).

The `Offset` parameter is used to determine the starting point for the lines to be retrieved. In this example, each request with a different `Offset` value fetches a new set of lines, allowing for controlled pagination through the dataset.

### Calculating Offset
To calculate the total number of pages and determine the appropriate `Offset` value for pagination, use the `GetTotalWarehousePickCount` method.

**Request:**
```json
{
  "ProcessMethod": "GetTotalWarehousePickCount",
  "Parameters": [
    {
      "No": "WHSE PICK-02826",
      "WarehouseEmployee": "ASIA1"
    }
  ]
}
```

**Response:**
```json
{
  "TotalCount": 8
}
```

### Steps to Calculate Offset
1. **Determine Total Count**: Use the `GetTotalWarehousePickCount` method to get the total number of lines (e.g., `TotalCount = 8`).
2. **Calculate Total Pages**: Divide the `TotalCount` by the `Limit` to get the total number of pages. If there is a remainder, round up to the next whole number.
   - Example: If `TotalCount = 8` and `Limit = 2`, then `TotalPages = 8 / 2 = 4`.
3. **Set Offset for Each Page**: The `Offset` value for each page can be calculated as `PageNumber`.
   - For Page 1: `Offset = 1`
   - For Page 2: `Offset = 2`
   - For Page 3: `Offset = 3`
   - For Page 4: `Offset = 4`

### Summary
The `GetPagedWarehousePick` method, with the use of `Limit` and `Offset` parameters, facilitates efficient data retrieval in a paginated manner. The `GetTotalWarehousePickCount` method can be used to determine the total number of lines, allowing for the calculation of the total number of pages and appropriate `Offset` values. Each subsequent `Offset` value ensures a new batch of lines is fetched, enabling easy management of large datasets.