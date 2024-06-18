**Request:**
```
{
  "ProcessMethod": "GetDayEndPayments",
  "Parameters": [
    {
      "SalesPerson": "JO",
      "Date": "2024-06-12",
    }
  ]
}
```
**Output:**
```
{
  "CompanyName": "ROE",
  "Date": "123",
  "SalesPerson": "JO",
  "Total": 3000,
  "PaymentDetail": [
    {
      "PaymentMethod": "CASH",
      "Total": 300,
      "Details": [
        {
          "DocumentNo": "G04037",
          "InvoiceNo": "INV-000001",
          "PostingDate": "2024-06-12",
          "Amount": 100,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        },
        {
          "DocumentNo": "G04037",
          "InvoiceNo": "INV-000002",
          "PostingDate": "2024-06-12",
          "Amount": 200,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        }
      ]
    },
    {
      "PaymentMethod": "CHECK",
      "Total": 60,
      "Details": [
        {
          "DocumentNo": "G04039",
          "InvoiceNo": "INV-000003",
          "PostingDate": "2024-06-12",
          "Amount": 50,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        },
        {
          "DocumentNo": "G04041",
          "InvoiceNo": "INV-000004",
          "PostingDate": "2024-06-12",
          "Amount": 10,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        }
      ]
    }
  ]
}
```

**Output:**
```
{
  "CompanyName": "MADISCO",
  "Date": "2024-06-12",
  "SalesPerson": "JO",
  "Total": 2387.2,
  "PaymentDetail": [
    {
      "PaymentMethod": "CASH",
      "Total": 2387.2,
      "Details": [
        {
          "DocumentNo": "G04037",
          "InvoiceNo": "G04037",
          "PostingDate": "2024-06-12",
          "Amount": 192.8,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        },
        {
          "DocumentNo": "G04037",
          "InvoiceNo": "G04037",
          "PostingDate": "2024-06-12",
          "Amount": 1000.8,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        },
        {
          "DocumentNo": "G04038",
          "InvoiceNo": "G04038",
          "PostingDate": "2024-06-12",
          "Amount": 1000.8,
          "Customer": {
            "No": "10000",
            "Name": "Adatum Corporation"
          }
        },
        {
          "DocumentNo": "G04038",
          "InvoiceNo": "G04038",
          "PostingDate": "2024-06-12",
          "Amount": 192.8,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        }
      ]
    }
  ],
  "Duration": "135 milliseconds"
}
```

