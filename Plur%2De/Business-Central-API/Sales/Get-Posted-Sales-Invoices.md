**ProcessMethod**: GetPostedSalesInvoice

**Description**:
Method that brings any Posted Sales Invoice

**Ouput**: 
-	**Posted Sales Invoice:** JsonArray with Posted Sales Invoice 1 or n 
**Example**:

Request:

One

`"jsonRequest":"{\"ProcessMethod\":\"GetPostedSalesInvoice\",\"Parameters\":[{\"No\":\"PS-INV103285\"}]}"`

**Outputs:**

```
{
  "SalesInvoice": {
    "SalesInvoiceHeader": [
      {
        "No": "PS-INV103285",
        "BilltoCustomerNo": "20000",
        "BilltoName": "Trey Research",
        "PostingDate": "2024-04-09",
        "DueDate": "2024-04-23",
        "LocationCode": "",
        "CurrencyCode": "",
        "OrderNo": "S-ORD101173",
        "AppliestoDocNo": "",
        "Amount": 192.8,
        "AmountIncludeVAT": 192.8,
        "SelltoAddress": "153 Thomas Drive",
        "SelltoCity": "Chicago",
        "PreAssignedNo": "",
        "RemainingAmount": 0.0,
        "Total": 192.8,
        "SalesInvoiceLines": [
          {
            "DocumentNo": "PS-INV103285",
            "LineNo": 1000,
            "Type": "Item",
            "No": "1900-S",
            "LocationCode": "EAST",
            "Description": "PARIS Guest Chair, black",
            "UnitofMeasure": "Piece",
            "Quantity": 1.0,
            "UnitPrice": 192.8,
            "VAT%": 0.0,
            "LineDiscount%": 0.0,
            "LineDiscountAmount": 0.0,
            "Amount": 192.8,
            "AmountIncludingVAT": 192.8,
            "GenBusPostingGroup": "DOMESTIC",
            "GenProdPostingGroup": "RETAIL",
            "VATBusPostingGroup": "",
            "VATProdPostingGroup": "",
            "VariantCode": "",
            "BinCode": ""
          }
        ]
      }
    ]
  }
}
```
Many

`"jsonRequest":"{\"ProcessMethod\":\"GetPostedSalesInvoice\",\"Parameters\":[{\"No\":\"PS-INV103285|PS-INV103284|PS-INV103283\"}]}"`

**Outputs:**

```
{
  "SalesInvoice": {
    "SalesInvoiceHeader": [
      {
        "No": "PS-INV103283",
        "BilltoCustomerNo": "10000",
        "BilltoName": "Adatum Corporation",
        "PostingDate": "2024-04-09",
        "DueDate": "2024-05-09",
        "LocationCode": "",
        "CurrencyCode": "",
        "OrderNo": "S-ORD101171",
        "AppliestoDocNo": "",
        "Amount": 192.8,
        "AmountIncludeVAT": 192.8,
        "SelltoAddress": "192 Market Square",
        "SelltoCity": "Atlanta",
        "PreAssignedNo": "",
        "RemainingAmount": 0.0,
        "Total": 192.8,
        "SalesInvoiceLines": [
          {
            "DocumentNo": "PS-INV103283",
            "LineNo": 1000,
            "Type": "Item",
            "No": "1900-S",
            "LocationCode": "EAST",
            "Description": "PARIS Guest Chair, black",
            "UnitofMeasure": "Piece",
            "Quantity": 1.0,
            "UnitPrice": 192.8,
            "VAT%": 0.0,
            "LineDiscount%": 0.0,
            "LineDiscountAmount": 0.0,
            "Amount": 192.8,
            "AmountIncludingVAT": 192.8,
            "GenBusPostingGroup": "DOMESTIC",
            "GenProdPostingGroup": "RETAIL",
            "VATBusPostingGroup": "",
            "VATProdPostingGroup": "",
            "VariantCode": "",
            "BinCode": ""
          }
        ]
      },
      {
        "No": "PS-INV103284",
        "BilltoCustomerNo": "10000",
        "BilltoName": "Adatum Corporation",
        "PostingDate": "2024-04-09",
        "DueDate": "2024-05-09",
        "LocationCode": "",
        "CurrencyCode": "",
        "OrderNo": "S-ORD101172",
        "AppliestoDocNo": "",
        "Amount": 192.8,
        "AmountIncludeVAT": 192.8,
        "SelltoAddress": "192 Market Square",
        "SelltoCity": "Atlanta",
        "PreAssignedNo": "",
        "RemainingAmount": 0.0,
        "Total": 192.8,
        "SalesInvoiceLines": [
          {
            "DocumentNo": "PS-INV103284",
            "LineNo": 1000,
            "Type": "Item",
            "No": "1900-S",
            "LocationCode": "EAST",
            "Description": "PARIS Guest Chair, black",
            "UnitofMeasure": "Piece",
            "Quantity": 1.0,
            "UnitPrice": 192.8,
            "VAT%": 0.0,
            "LineDiscount%": 0.0,
            "LineDiscountAmount": 0.0,
            "Amount": 192.8,
            "AmountIncludingVAT": 192.8,
            "GenBusPostingGroup": "DOMESTIC",
            "GenProdPostingGroup": "RETAIL",
            "VATBusPostingGroup": "",
            "VATProdPostingGroup": "",
            "VariantCode": "",
            "BinCode": ""
          }
        ]
      },
      {
        "No": "PS-INV103285",
        "BilltoCustomerNo": "20000",
        "BilltoName": "Trey Research",
        "PostingDate": "2024-04-09",
        "DueDate": "2024-04-23",
        "LocationCode": "",
        "CurrencyCode": "",
        "OrderNo": "S-ORD101173",
        "AppliestoDocNo": "",
        "Amount": 192.8,
        "AmountIncludeVAT": 192.8,
        "SelltoAddress": "153 Thomas Drive",
        "SelltoCity": "Chicago",
        "PreAssignedNo": "",
        "RemainingAmount": 0.0,
        "Total": 192.8,
        "SalesInvoiceLines": [
          {
            "DocumentNo": "PS-INV103285",
            "LineNo": 1000,
            "Type": "Item",
            "No": "1900-S",
            "LocationCode": "EAST",
            "Description": "PARIS Guest Chair, black",
            "UnitofMeasure": "Piece",
            "Quantity": 1.0,
            "UnitPrice": 192.8,
            "VAT%": 0.0,
            "LineDiscount%": 0.0,
            "LineDiscountAmount": 0.0,
            "Amount": 192.8,
            "AmountIncludingVAT": 192.8,
            "GenBusPostingGroup": "DOMESTIC",
            "GenProdPostingGroup": "RETAIL",
            "VATBusPostingGroup": "",
            "VATProdPostingGroup": "",
            "VariantCode": "",
            "BinCode": ""
          }
        ]
      }
    ]
  }
}
```
