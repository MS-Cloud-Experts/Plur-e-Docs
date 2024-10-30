### API Documentation: GetSalesOrders

#### Overview
The `GetSalesOrders` API method retrieves a list of sales orders associated with a specified salesperson, enabling users to access detailed sales order information, including customer details, billing and shipping addresses, and itemized order lines. This API supports efficient order management and tracking for sales and logistics teams.

#### Request Structure
```json
{
  "ProcessMethod": "GetSalesOrders",
  "Parameters": [
    {
      "type": "Sales Order",
      "pageSize": "",
      "position": "",
      "salesPerson": "BC"
    }
  ]
}
```

#### Parameters
- **type**: Specifies the type of document to retrieve, in this case, `"Sales Order"`.
- **pageSize**: Optional. Determines the number of records returned per page.
- **position**: Optional. Identifies the position from which to retrieve records, useful for pagination.
- **salesPerson**: The code of the salesperson associated with the orders to be retrieved (e.g., `"BC"`).

#### Example Request
```json
{
  "ProcessMethod": "GetSalesOrders",
  "Parameters": [
    {
      "type": "Sales Order",
      "pageSize": "",
      "position": "",
      "salesPerson": "BC"
    }
  ]
}
```

#### Example Response
```json
{
  "SalesOrders": [
    {
      "id": 36,
      "name": "SalesHeader",
      "company": "CRONUS USA, Inc.",
      "position": "Document Type=CONST(Order),No.=CONST(S-ORD101032)",
      "recordId": "Sales Header: Order,S-ORD101032",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "DocumentType",
            "type": "Option",
            "value": "Order",
            "System": true
          },
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "S-ORD101032",
            "System": true
          }
        ]
      },
      "fields": [
        {"id": 2, "name": "SelltoCustomerNo", "type": "Code", "value": "20000"},
        {"id": 5, "name": "BilltoName", "type": "Text", "value": "Trey Research"},
        {"id": 7, "name": "BilltoAddress", "type": "Text", "value": "153 Thomas Drive"},
        {"id": 19, "name": "OrderDate", "type": "Date", "value": "2024-10-28"},
        {"id": 43, "name": "SalespersonCode", "type": "Code", "value": "BC"},
        {"id": 60, "name": "Amount", "type": "Decimal", "value": null},
        {"id": 120, "name": "Status", "type": "Option", "value": "Open"}
      ],
      "SalesLines": [
        {
          "id": 37,
          "name": "SalesLine",
          "position": "Document Type=CONST(Order),Document No.=CONST(S-ORD101032),Line No.=CONST(1000)",
          "fields": [
            {"id": 6, "name": "No", "type": "Code", "value": "1001"},
            {"id": 15, "name": "Quantity", "type": "Decimal", "value": 1.0},
            {"id": 22, "name": "UnitPrice", "type": "Decimal", "value": null},
            {"id": 29, "name": "Amount", "type": "Decimal", "value": null}
          ]
        }
      ]
    }
    // Additional sales orders omitted for brevity
  ]
}
```

#### Explanation
- **SalesOrders**: An array of objects representing individual sales orders. Each object contains:
  - **id**: Unique identifier of the sales order.
  - **company**: The name of the company associated with the sales order.
  - **position**: Specifies the document type and order number.
  - **recordId**: A unique identifier string for the sales header.
  - **fields**: An array of field objects detailing order information such as customer number, order date, salesperson code, amount, and status.
- **SalesLines**: Nested within each sales order, this array contains details of each item on the sales order, with fields like item number, quantity, unit price, and amount.

#### Summary
The `GetSalesOrders` API provides structured access to comprehensive sales order information for efficient order processing and inventory management. By capturing details such as billing information, order lines, quantities, and pricing, this method supports effective sales tracking and facilitates decision-making processes in sales and logistics.