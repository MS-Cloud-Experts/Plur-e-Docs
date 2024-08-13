### API Documentation: GetSalesDocumentsBySalesPerson

#### Overview
The `GetSalesDocumentsBySalesPerson` API method retrieves detailed sales document information based on the specified Sales Person, Start Date, and End Date. The method returns data from multiple sales document types, including Sales Orders, Sales Invoices, Sales Credit Memos, Sales Return Orders, Posted Sales Invoices, and Posted Sales Credit Memos. The API provides a structured JSON response that includes key information such as Document Type, Amount, and Posting Date, allowing for comprehensive analysis of sales activities for the given Sales Person.

#### Request Structure
```json
{
  "ProcessMethod": "GetSalesDocumentsBySalesPerson",
  "Parameters": [
    {
      "SalesPersonCode": "SP001",
      "StartDate": "2024-01-01",
      "EndDate": "2024-01-31"
    }
  ]
}
```

#### Parameters
- **SalesPersonCode**: The code identifying the Sales Person (e.g., `"SP001"`).
- **StartDate**: The start date of the period for which to retrieve sales documents (e.g., `"2024-01-01"`).
- **EndDate**: The end date of the period for which to retrieve sales documents (e.g., `"2024-01-31"`).

#### Example Request
```json
{
  "ProcessMethod": "GetSalesDocumentsBySalesPerson",
  "Parameters": [
    {
      "SalesPersonCode": "SP001",
      "StartDate": "2024-01-01",
      "EndDate": "2024-01-31"
    }
  ]
}
```

#### Example Response
```json
{
  "Documents": [
    {
      "Document Type": "Sales Order",
      "Amount": 1500.00,
      "Posting Date": "2024-01-05"
    },
    {
      "Document Type": "Sales Invoice",
      "Amount": 2000.00,
      "Posting Date": "2024-01-10"
    },
    {
      "Document Type": "Sales Credit Memo",
      "Amount": -500.00,
      "Posting Date": "2024-01-15"
    },
    {
      "Document Type": "Posted Sales Invoice",
      "Amount": 2500.00,
      "Posting Date": "2024-01-20"
    },
    {
      "Document Type": "Posted Sales Credit Memo",
      "Amount": -300.00,
      "Posting Date": "2024-01-25"
    }
  ]
}
```

#### Explanation
- **Documents**: An array containing objects for each sales document retrieved based on the Sales Person and date range specified.
  - **Document Type**: The type of the sales document (e.g., `"Sales Order"`, `"Sales Invoice"`, `"Sales Credit Memo"`, `"Sales Return Order"`, `"Posted Sales Invoice"`, `"Posted Sales Credit Memo"`).
  - **Amount**: The amount associated with the document (e.g., `1500.00`).
  - **Posting Date**: The date when the document was posted (e.g., `"2024-01-05"`).

#### Summary
The `GetSalesDocumentsBySalesPerson` method allows for retrieving a comprehensive set of sales documents related to a specific Sales Person within a defined date range. This API is essential for sales tracking and reporting, enabling users to gather detailed insights into sales performance, document activities, and financial outcomes for the specified period. The response is structured to support further analysis and integration into broader sales management systems within Business Central.