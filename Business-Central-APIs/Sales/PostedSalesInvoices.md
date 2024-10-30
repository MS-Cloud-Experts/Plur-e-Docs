### API Documentation: PostedSalesInvoices

#### Overview
The `PostedSalesInvoices` API method retrieves a list of posted sales invoices based on specified criteria, including date range, salesperson, and customer number. This provides access to detailed sales invoice information, such as billing details, amounts, and itemized invoice lines, which assists in financial tracking and customer account management.

#### Request Structure
```json
{
  "ProcessMethod": "PostedSalesInvoices",
  "Parameters": [
    {
      "Open": true,
      "StartDate": "2024-10-21",
      "EndDate": "2024-10-21",
      "salesPerson": "BC",
      "CustomerNo": ""
    }
  ]
}
```

#### Parameters
- **Open**: Boolean value indicating whether to retrieve only open (unpaid) invoices.
- **StartDate**: Start date of the range for invoice posting dates (e.g., `"2024-10-21"`).
- **EndDate**: End date of the range for invoice posting dates (e.g., `"2024-10-21"`).
- **salesPerson**: The code of the salesperson associated with the invoices.
- **CustomerNo**: Optional. The customer number for which invoices are requested; leave blank to retrieve invoices for all customers within the specified criteria.

#### Example Request
```json
{
  "ProcessMethod": "PostedSalesInvoices",
  "Parameters": [
    {
      "Open": true,
      "StartDate": "2024-10-21",
      "EndDate": "2024-10-21",
      "salesPerson": "BC",
      "CustomerNo": ""
    }
  ]
}
```

#### Example Response
```json
{
  "SalesOrders": [
    {
      "id": 112,
      "name": "SalesInvoiceHeader",
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103219)",
      "recordId": "Sales Invoice Header: PS-INV103219",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103219",
            "System": true
          }
        ]
      },
      "fields": [
        {"id": 4, "name": "BilltoCustomerNo", "type": "Code", "value": "10000"},
        {"id": 5, "name": "BilltoName", "type": "Text", "value": "Adatum Corporation"},
        {"id": 20, "name": "PostingDate", "type": "Date", "value": "2024-10-29"},
        {"id": 24, "name": "DueDate", "type": "Date", "value": "2024-11-29"},
        {"id": 60, "name": "Amount", "type": "Decimal", "value": 2001.6},
        {"id": 61, "name": "AmountIncludingVAT", "type": "Decimal", "value": 2001.6}
      ],
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "position": "Document No.=CONST(PS-INV103219),Line No.=CONST(10000)",
          "fields": [
            {"id": 6, "name": "No", "type": "Code", "value": "1896-S"},
            {"id": 11, "name": "Description", "type": "Text", "value": "ATHENS Desk"},
            {"id": 15, "name": "Quantity", "type": "Decimal", "value": 2.0},
            {"id": 22, "name": "UnitPrice", "type": "Decimal", "value": 1000.8},
            {"id": 29, "name": "Amount", "type": "Decimal", "value": 2001.6}
          ]
        }
      ]
    }
    // Additional sales invoices omitted for brevity
  ],
  "Information": "The client does not have expired orders."
}
```

#### Explanation
- **SalesOrders**: Array of sales invoice objects based on the criteria specified in the request.
  - **id**: Unique identifier for each sales invoice.
  - **company**: The company associated with the invoice.
  - **fields**: Array containing key details like customer number, invoice amount, posting date, due date, and VAT-inclusive amount.
  - **SalesLines**: Array representing the lines on each invoice, with details including:
    - **No**: Item code on the invoice.
    - **Description**: Item description.
    - **Quantity** and **UnitPrice**: Quantity sold and unit price.
    - **Amount**: Total amount for the line.
- **Information**: Message indicating any relevant status, such as whether there are expired or open invoices.

#### Summary
The `PostedSalesInvoices` API method provides detailed data on posted sales invoices within a defined date range, supporting financial and customer account management. By capturing essential invoice details, it enables sales and finance teams to track payments, manage outstanding invoices, and review specific transaction details with customers.