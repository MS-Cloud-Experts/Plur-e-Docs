**Request:**
```
{
  "ProcessMethod": "GetPaymentReceipt",
  "Parameters": [
    {
      "DocumentNo": "PS-INV103192"
    }
  ]
}
```

**Output:**
```
{
  "InvoiceNumber": "PS-INV103192",
  "PostingDate": "2023-03-25",
  "Amount": -4596.16,
  "Customer": {
    "No": "50000",
    "Name": "Relecloud",
    "Address1": "25 Water Way",
    "Address2": "",
    "City": "Atlanta",
    "CountryRegionCode": "US",
    "PostCode": "31772",
    "ResponsibilityCenter": "",
    "PaymentMethodCode": ""
  },
  "SalesPerson": {
    "Code": "JO",
    "Name": "Jim Olive"
  },
  "CompanyInfo": {
    "Name": "Adventure DEV",
    "Address1": "7122 South Ashford Street",
    "Address2": "Westminster",
    "City": "Atlanta",
    "CountryRegionCode": "US",
    "PostCode": "31772",
    "TIN": "",
    "PhoneNo": "+1 425 555 0100"
  },
  "PostedSalesInvoice": "PS-INV103192"
}
```
**Document in Business Central:**
![image.png](/.attachments/image-135ccb9f-dbe4-4ffb-abf1-cd29b1950239.png)

**Payment Receipt**
![image.png](/.attachments/image-2cca1580-3db4-4679-92d0-46b2dc6e86f8.png)