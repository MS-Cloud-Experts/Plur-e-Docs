### API Documentation: GetSalesDocumentsBySalesPerson

#### Overview
The `GetSalesDocumentsBySalesPerson` API method retrieves detailed sales document information based on the specified Sales Person, Start Date, and End Date. 

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
      "Sales Order": [
        {
          "Document Type": "Sales Order",
          "Amount": 1500.0,
          "Posting Date": "2024-01-05"
        }
      ]
    },
    {
      "Sales Invoice": [
        {
          "Document Type": "Sales Invoice",
          "Amount": 2000.0,
          "Posting Date": "2024-01-10"
        }
      ]
    },
    {
      "Sales Credit Memo": [
        {
          "Document Type": "Sales Credit Memo",
          "Amount": -500.0,
          "Posting Date": "2024-01-15"
        }
      ]
    },
    {
      "Sales Return Order": [
        {
          "Document Type": "Sales Return Order",
          "Amount": 1000.0,
          "Posting Date": "2024-01-12"
        }
      ]
    },
    {
      "Posted Sales Invoice": [
        {
          "Document Type": "Posted Sales Invoice",
          "Amount": 2500.0,
          "Posting Date": "2024-01-20"
        }
      ]
    },
    {
      "Posted Sales Credit Memo": [
        {
          "Document Type": "Posted Sales Credit Memo",
          "Amount": -300.0,
          "Posting Date": "2024-01-25"
        }
      ]
    }
  ]
}
```

#### Explanation
- **Documents**: The main array containing groups of sales documents organized by type.
  - **Sales Order, Sales Invoice, Sales Credit Memo, Sales Return Order, Posted Sales Invoice, Posted Sales Credit Memo**: Each type of document is represented as an array of objects within the `Documents` array.
    - **Document Type**: The type of the sales document (e.g., `"Sales Order"`, `"Sales Invoice"`, etc.).
    - **Amount**: The amount associated with the document (e.g., `1500.0`).
    - **Posting Date**: The date when the document was posted (e.g., `"2024-01-05"`).

#### Summary
The `GetSalesDocumentsBySalesPerson` method organizes sales documents by type, providing a clear and detailed JSON response for the specified Sales Person and date range. This structure enables efficient analysis and integration into sales reporting systems, supporting enhanced decision-making processes within Business Central.