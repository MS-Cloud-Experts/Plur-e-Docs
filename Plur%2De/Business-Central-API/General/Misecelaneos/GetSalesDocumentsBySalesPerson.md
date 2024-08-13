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
          "DocumentNo": "SOB2B-302997",
          "Amount": 2055.06,
          "Posting Date": "2024-07-24"
        }
      ]
    },
    {
      "Sales Invoice": []
    },
    {
      "Sales Credit Memo": []
    },
    {
      "Sales Return Order": [
        {
          "DocumentNo": "SRR-119471",
          "Amount": 0.0,
          "Posting Date": "2024-06-11"
        }
      ]
    },
    {
      "Posted Sales Invoice": [
        {
          "DocumentNo": "SINP-129091",
          "Amount": 538.0,
          "Posting Date": "2024-03-06"
        },
        {
          "DocumentNo": "SINP-130527",
          "Amount": 4053.15,
          "Posting Date": "2024-04-30"
        },
        {
          "DocumentNo": "SINP-130592",
          "Amount": 2146.88,
          "Posting Date": "2024-05-01"
        },
        {
          "DocumentNo": "SINP-130785",
          "Amount": 120.05,
          "Posting Date": "2024-05-13"
        },
        {
          "DocumentNo": "SINP-130787",
          "Amount": 1304.04,
          "Posting Date": "2024-05-13"
        },
        {
          "DocumentNo": "SINP-130858",
          "Amount": 375.0,
          "Posting Date": "2024-05-15"
        },
        {
          "DocumentNo": "SINP-131036",
          "Amount": 1059.0,
          "Posting Date": "2024-05-24"
        },
        {
          "DocumentNo": "SINP-131208",
          "Amount": 31.6,
          "Posting Date": "2024-06-03"
        },
        {
          "DocumentNo": "SINP-131265",
          "Amount": 1419.0,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SINP-131357",
          "Amount": 83.92,
          "Posting Date": "2024-06-10"
        },
        {
          "DocumentNo": "SINP-131391",
          "Amount": 529.5,
          "Posting Date": "2024-06-12"
        },
        {
          "DocumentNo": "SINP-131452",
          "Amount": 982.14,
          "Posting Date": "2024-06-14"
        },
        {
          "DocumentNo": "SINP-131516",
          "Amount": 51.12,
          "Posting Date": "2024-06-18"
        },
        {
          "DocumentNo": "SINP-131702",
          "Amount": 993.5,
          "Posting Date": "2024-06-27"
        },
        {
          "DocumentNo": "SINP-131824",
          "Amount": 499.5,
          "Posting Date": "2024-07-09"
        },
        {
          "DocumentNo": "SINP-131905",
          "Amount": 2651.25,
          "Posting Date": "2024-07-12"
        },
        {
          "DocumentNo": "SINP-132008",
          "Amount": 389.0,
          "Posting Date": "2024-07-16"
        },
        {
          "DocumentNo": "SINP-132024",
          "Amount": 739.5,
          "Posting Date": "2024-07-22"
        },
        {
          "DocumentNo": "SINP-132085",
          "Amount": 2258.9,
          "Posting Date": "2024-07-22"
        }
      ]
    },
    {
      "Posted Sales Credit Memo": [
        {
          "DocumentNo": "SINP-132085",
          "Amount": 1208.0,
          "Posting Date": "2024-05-13"
        },
        {
          "DocumentNo": "SINP-132085",
          "Amount": 29.4,
          "Posting Date": "2024-06-10"
        },
        {
          "DocumentNo": "SINP-132085",
          "Amount": 499.5,
          "Posting Date": "2024-06-14"
        },
        {
          "DocumentNo": "SINP-132085",
          "Amount": 549.45,
          "Posting Date": "2024-07-08"
        },
        {
          "DocumentNo": "SINP-132085",
          "Amount": 1710.1,
          "Posting Date": "2024-07-11"
        },
        {
          "DocumentNo": "SINP-132085",
          "Amount": 454.0,
          "Posting Date": "2024-07-15"
        }
      ]
    }
  ],
  "Duration": "132 milliseconds"
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