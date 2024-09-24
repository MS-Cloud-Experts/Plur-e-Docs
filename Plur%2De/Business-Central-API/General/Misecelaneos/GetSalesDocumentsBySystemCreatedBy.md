### API Documentation: GetSalesDocumentsBySystemCreatedBy

#### Overview
The `GetSalesDocumentsBySystemCreatedBy` API method retrieves detailed sales document information based on the specified Creator User, Start Date, and End Date. 

#### Request Structure
```json
{
  "ProcessMethod": "GetSalesDocumentsBySystemCreatedBy",
  "Parameters": [
    {
      "CreateBy": "PANGEA",
      "SalesPersonCode": "",
      "StartDate": "2024-01-01",
      "EndDate": "2024-12-31"
    }
  ]
} 
```

#### Parameters
- **CreateBy**: The code identifying the user who created the document (e.g., `"PANGEA"`).
- **SalesPersonCode**: The code identifying the Sales Person (e.g., `"SP001"`).
- **StartDate**: The start date of the period for which to retrieve sales documents (e.g., `"2024-01-01"`).
- **EndDate**: The end date of the period for which to retrieve sales documents (e.g., `"2024-01-31"`).

#### Example Request
```json
{
  "ProcessMethod": "GetSalesDocumentsBySystemCreatedBy",
  "Parameters": [
    {
      "CreateBy": "PANGEA",
      "SalesPersonCode": "",
      "StartDate": "2024-01-01",
      "EndDate": "2024-12-31"
    }
  ]
} 
```

#### Example Response
```json
{
  "Documents": [
    {
      "Sales Orders": [
        {
          "DocumentNo": "SO-418162",
          "Amount": 61.3,
          "Posting Date": "2024-03-18"
        },
        {
          "DocumentNo": "SO-418163",
          "Amount": 61.31,
          "Posting Date": "2024-03-18"
        },
        {
          "DocumentNo": "SO-418164",
          "Amount": 122.61,
          "Posting Date": "2024-03-18"
        },
        {
          "DocumentNo": "SO-418165",
          "Amount": 48.93,
          "Posting Date": "2024-03-18"
        },
        {
          "DocumentNo": "SO-418166",
          "Amount": 1.0,
          "Posting Date": "2024-03-27"
        },
        {
          "DocumentNo": "SO-418167",
          "Amount": 1.0,
          "Posting Date": "2024-03-27"
        },
        {
          "DocumentNo": "SO-418168",
          "Amount": 1.0,
          "Posting Date": "2024-04-09"
        },
        {
          "DocumentNo": "SO-418174",
          "Amount": 35.75,
          "Posting Date": "2024-05-02"
        },
        {
          "DocumentNo": "SO-418175",
          "Amount": 35.75,
          "Posting Date": "2024-05-02"
        },
        {
          "DocumentNo": "SO-418206",
          "Amount": 336.02,
          "Posting Date": "2024-05-24"
        },
        {
          "DocumentNo": "SO-418210",
          "Amount": 0.0,
          "Posting Date": "2024-05-29"
        },
        {
          "DocumentNo": "SO-418211",
          "Amount": 35.75,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SO-418212",
          "Amount": 35.75,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SO-418213",
          "Amount": 35.75,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SO-418214",
          "Amount": 35.75,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SO-418215",
          "Amount": 35.75,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SO-418216",
          "Amount": 35.75,
          "Posting Date": "2024-06-05"
        },
        {
          "DocumentNo": "SO-418225",
          "Amount": 58.33,
          "Posting Date": "2024-06-17"
        },
        {
          "DocumentNo": "SO-418226",
          "Amount": 58.33,
          "Posting Date": "2024-06-17"
        },
        {
          "DocumentNo": "SO-418227",
          "Amount": 35.75,
          "Posting Date": "2024-06-25"
        },
        {
          "DocumentNo": "SO-418228",
          "Amount": 35.75,
          "Posting Date": "2024-06-25"
        },
        {
          "DocumentNo": "SO-418229",
          "Amount": 35.75,
          "Posting Date": "2024-06-25"
        },
        {
          "DocumentNo": "SO-418230",
          "Amount": 35.75,
          "Posting Date": "2024-06-25"
        },
        {
          "DocumentNo": "SO-418231",
          "Amount": 36.75,
          "Posting Date": "2024-06-25"
        },
        {
          "DocumentNo": "SO-418232",
          "Amount": 35.75,
          "Posting Date": "2024-07-02"
        },
        {
          "DocumentNo": "SO-418233",
          "Amount": 35.75,
          "Posting Date": "2024-07-02"
        },
        {
          "DocumentNo": "SO-418234",
          "Amount": 71.5,
          "Posting Date": "2024-07-02"
        },
        {
          "DocumentNo": "SO-418235",
          "Amount": 35.75,
          "Posting Date": "2024-07-02"
        },
        {
          "DocumentNo": "SO-418236",
          "Amount": 35.75,
          "Posting Date": "2024-07-02"
        },
        {
          "DocumentNo": "SO-418237",
          "Amount": 0.0,
          "Posting Date": "2024-07-03"
        },
        {
          "DocumentNo": "SO-418238",
          "Amount": 1.0,
          "Posting Date": "2024-06-26"
        },
        {
          "DocumentNo": "SO-418239",
          "Amount": 1.0,
          "Posting Date": "2024-06-26"
        },
        {
          "DocumentNo": "SO-418240",
          "Amount": 1.5,
          "Posting Date": "2024-07-03"
        },
        {
          "DocumentNo": "SO-418241",
          "Amount": 35.75,
          "Posting Date": "2024-07-03"
        },
        {
          "DocumentNo": "SO-418246",
          "Amount": 35.75,
          "Posting Date": "2024-07-09"
        },
        {
          "DocumentNo": "SO-418247",
          "Amount": 35.75,
          "Posting Date": "2024-07-09"
        },
        {
          "DocumentNo": "SO-418248",
          "Amount": 35.75,
          "Posting Date": "2024-07-09"
        },
        {
          "DocumentNo": "SO-418253",
          "Amount": 307.7,
          "Posting Date": "2024-07-17"
        },
        {
          "DocumentNo": "SO-418256",
          "Amount": 35.75,
          "Posting Date": "2024-07-17"
        },
        {
          "DocumentNo": "SO-418257",
          "Amount": 35.75,
          "Posting Date": "2024-07-18"
        },
        {
          "DocumentNo": "SO-418261",
          "Amount": 0.0,
          "Posting Date": "2024-07-31"
        },
        {
          "DocumentNo": "SO-418262",
          "Amount": 0.0,
          "Posting Date": "2024-07-31"
        },
        {
          "DocumentNo": "SO-418266",
          "Amount": 35.75,
          "Posting Date": "2024-08-06"
        }
      ],
      "Total": 43.0
    },
    {
      "Sales Invoice": [
        {
          "DocumentNo": "SI-203190",
          "Amount": 61.3,
          "Posting Date": "2024-03-18"
        },
        {
          "DocumentNo": "SI-203191",
          "Amount": 0.01,
          "Posting Date": "2024-07-18"
        },
        {
          "DocumentNo": "SI-203193",
          "Amount": 5344.09,
          "Posting Date": "2024-05-23"
        },
        {
          "DocumentNo": "SI-203194",
          "Amount": 35.75,
          "Posting Date": "2024-06-06"
        },
        {
          "DocumentNo": "SI-203197",
          "Amount": 0.0,
          "Posting Date": "2024-07-03"
        },
        {
          "DocumentNo": "SI-203203",
          "Amount": 213.36,
          "Posting Date": "2024-07-13"
        },
        {
          "DocumentNo": "SI-203204",
          "Amount": 58.11,
          "Posting Date": "2024-07-13"
        }
      ],
      "Total": 7.0
    },
    {
      "Sales Credit Memo": [
        {
          "DocumentNo": "SCR-10997",
          "Amount": 35.75,
          "Posting Date": "2024-06-06"
        },
        {
          "DocumentNo": "SCR-10998",
          "Amount": 0.0,
          "Posting Date": "2024-07-03"
        }
      ],
      "Total": 2.0
    },
    {
      "Sales Return Order": [
        {
          "DocumentNo": "PSR-1039823",
          "Amount": 61.31,
          "Posting Date": "2024-03-18"
        },
        {
          "DocumentNo": "PSR-1039824",
          "Amount": 35.75,
          "Posting Date": "2024-06-06"
        },
        {
          "DocumentNo": "PSR-1039827",
          "Amount": 0.0,
          "Posting Date": "2024-07-03"
        }
      ],
      "Total": 3.0
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
The `GetSalesDocumentsBySystemCreatedBy` method organizes sales documents by type, providing a clear and detailed JSON response for the specified Creator User and date range. This structure enables efficient analysis and integration into sales reporting systems, supporting enhanced decision-making processes within Business Central.