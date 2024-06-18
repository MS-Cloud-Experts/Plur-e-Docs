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
  "CompanyName": "MADISCO",
  "Date": "2024-06-18",
  "SalesPerson": "JO",
  "Total": 4856.98,
  "PaymentDetail": [
    {
      "PaymentMethod": "CASH",
      "Total": 4636.96,
      "Details": [
        {
          "DocumentNo": "G04039",
          "InvoiceNo": "PS-INV103270",
          "PostingDate": "2024-06-18",
          "Amount": 433.6,
          "Customer": {
            "No": "10000",
            "Name": "Adatum Corporation"
          }
        },
        {
          "DocumentNo": "G04040",
          "InvoiceNo": "PS-INV103303",
          "PostingDate": "2024-06-18",
          "Amount": 4203.36,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        }
      ]
    },
    {
      "PaymentMethod": "CHECK",
      "Total": 220.02,
      "Details": [
        {
          "DocumentNo": "G04043",
          "InvoiceNo": "PS-INV103261",
          "PostingDate": "2024-06-18",
          "Amount": 220.02,
          "Customer": {
            "No": "10000",
            "Name": "Adatum Corporation"
          }
        }
      ]
    }
  ],
  "Duration": "18 seconds 586 milliseconds"
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

