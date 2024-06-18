**Request:**
```
{
  "ProcessMethod": "GetPaymentDocuments",
  "Parameters": []
}
```


```
{
  "Payments": [
    {
      "DocumentNo": "PS-INV103001",
      "PostingDate": "2022-01-18",
      "Amount": -172.94,
      "Customer": {
        "No": "20000",
        "Name": "Trey Research"
      },
      "ClosedByEntry": {
        "PostedSalesInvoice": "PS-INV103001"
      }
    },
    {
      "DocumentNo": "PS-INV103002",
      "PostingDate": "2022-01-19",
      "Amount": -817.47,
      "Customer": {
        "No": "10000",
        "Name": "Adatum Corporation"
      },
      "ClosedByEntry": {
        "PostedSalesInvoice": "PS-INV103002"
      }
    },
    {
      "DocumentNo": "PS-INV103003",
      "PostingDate": "2022-01-20",
      "Amount": -206.3,
      "Customer": {
        "No": "30000",
        "Name": "School of Fine Art"
      },
      "ClosedByEntry": {
        "PostedSalesInvoice": "PS-INV103003"
      }
    }
  ]
}
```
