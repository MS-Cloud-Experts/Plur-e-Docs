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
          "InvoiceNo": "PS-INV103285",
          "PostingDate": "2024-06-12",
          "Amount": 192.8,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        },
        {
          "DocumentNo": "G04037",
          "InvoiceNo": "PS-INV103297",
          "PostingDate": "2024-06-12",
          "Amount": 1000.8,
          "Customer": {
            "No": "20000",
            "Name": "Trey Research"
          }
        },
        {
          "DocumentNo": "G04038",
          "InvoiceNo": "PS-INV103276",
          "PostingDate": "2024-06-12",
          "Amount": 1000.8,
          "Customer": {
            "No": "10000",
            "Name": "Adatum Corporation"
          }
        },
        {
          "DocumentNo": "G04038",
          "InvoiceNo": "PS-INV103281",
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
  "Duration": "71 milliseconds"
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

