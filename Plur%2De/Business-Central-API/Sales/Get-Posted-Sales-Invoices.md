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
  "SalesOrders": [
    {
      "id": 112,
      "name": "SalesInvoiceHeader",
      "company": "Adventure",
      "position": "No.=CONST(PS-INV103285)",
      "recordId": "Sales Invoice Header: PS-INV103285",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103285",
            "System": true
          }
        ]
      },
      "fieldCount": 15,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103285",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "20000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Trey Research",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2024-04-09",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2024-04-23",
          "System": true
        },
        {
          "id": 28,
          "name": "LocationCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 32,
          "name": "CurrencyCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 44,
          "name": "OrderNo",
          "type": "Code",
          "value": "S-ORD101173",
          "System": true
        },
        {
          "id": 53,
          "name": "AppliestoDocNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 60,
          "name": "Amount",
          "type": "Decimal",
          "value": 192.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 192.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "153 Thomas Drive",
          "System": true
        },
        {
          "id": 83,
          "name": "SelltoCity",
          "type": "Text",
          "value": "Chicago",
          "System": true
        },
        {
          "id": 111,
          "name": "PreAssignedNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 1303,
          "name": "RemainingAmount",
          "type": "Decimal",
          "value": 192.8,
          "System": false
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "Adventure",
          "position": "Document No.=CONST(PS-INV103285),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103285,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103285",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 1000,
                "System": true
              }
            ]
          },
          "fieldCount": 20,
          "fields": [
            {
              "id": 3,
              "name": "DocumentNo",
              "type": "Code",
              "value": "PS-INV103285",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 1000,
              "System": true
            },
            {
              "id": 5,
              "name": "Type",
              "type": "Option",
              "value": "Item",
              "System": true
            },
            {
              "id": 6,
              "name": "No",
              "type": "Code",
              "value": "1900-S",
              "System": true
            },
            {
              "id": 7,
              "name": "LocationCode",
              "type": "Code",
              "value": "EAST",
              "System": true
            },
            {
              "id": 11,
              "name": "Description",
              "type": "Text",
              "value": "PARIS Guest Chair, black",
              "System": true
            },
            {
              "id": 13,
              "name": "UnitofMeasure",
              "type": "Text",
              "value": "Piece",
              "System": true
            },
            {
              "id": 15,
              "name": "Quantity",
              "type": "Decimal",
              "value": 1.0,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 25,
              "name": "VAT%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 27,
              "name": "LineDiscount%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 28,
              "name": "LineDiscountAmount",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 29,
              "name": "Amount",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 74,
              "name": "GenBusPostingGroup",
              "type": "Code",
              "value": "DOMESTIC",
              "System": true
            },
            {
              "id": 75,
              "name": "GenProdPostingGroup",
              "type": "Code",
              "value": "RETAIL",
              "System": true
            },
            {
              "id": 89,
              "name": "VATBusPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 90,
              "name": "VATProdPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5402,
              "name": "VariantCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5403,
              "name": "BinCode",
              "type": "Code",
              "value": null,
              "System": true
            }
          ]
        }
      ]
    }
  ]
}
```
Many

`"jsonRequest":"{\"ProcessMethod\":\"GetPostedSalesInvoice\",\"Parameters\":[{\"No\":\"PS-INV103285|PS-INV103223|PS-INV103197\"}]}"`

**Outputs:**

```
{
  "SalesOrders": [
    {
      "id": 112,
      "name": "SalesInvoiceHeader",
      "company": "Adventure",
      "position": "No.=CONST(PS-INV103197)",
      "recordId": "Sales Invoice Header: PS-INV103197",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103197",
            "System": true
          }
        ]
      },
      "fieldCount": 15,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103197",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "50000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Relecloud",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-03-31",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-04-14",
          "System": true
        },
        {
          "id": 28,
          "name": "LocationCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 32,
          "name": "CurrencyCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 44,
          "name": "OrderNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 53,
          "name": "AppliestoDocNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 60,
          "name": "Amount",
          "type": "Decimal",
          "value": 2907.4,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 3081.84,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "25 Water Way",
          "System": true
        },
        {
          "id": 83,
          "name": "SelltoCity",
          "type": "Text",
          "value": "Atlanta",
          "System": true
        },
        {
          "id": 111,
          "name": "PreAssignedNo",
          "type": "Code",
          "value": "S-INV102197",
          "System": true
        },
        {
          "id": 1303,
          "name": "RemainingAmount",
          "type": "Decimal",
          "value": 3081.84,
          "System": false
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "Adventure",
          "position": "Document No.=CONST(PS-INV103197),Line No.=CONST(10000)",
          "recordId": "Sales Invoice Line: PS-INV103197,10000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103197",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 10000,
                "System": true
              }
            ]
          },
          "fieldCount": 20,
          "fields": [
            {
              "id": 3,
              "name": "DocumentNo",
              "type": "Code",
              "value": "PS-INV103197",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 10000,
              "System": true
            },
            {
              "id": 5,
              "name": "Type",
              "type": "Option",
              "value": "Item",
              "System": true
            },
            {
              "id": 6,
              "name": "No",
              "type": "Code",
              "value": "1920-S",
              "System": true
            },
            {
              "id": 7,
              "name": "LocationCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 11,
              "name": "Description",
              "type": "Text",
              "value": "ANTWERP Conference Table",
              "System": true
            },
            {
              "id": 13,
              "name": "UnitofMeasure",
              "type": "Text",
              "value": "Piece",
              "System": true
            },
            {
              "id": 15,
              "name": "Quantity",
              "type": "Decimal",
              "value": 3.0,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 647.8,
              "System": true
            },
            {
              "id": 25,
              "name": "VAT%",
              "type": "Decimal",
              "value": 6.0,
              "System": true
            },
            {
              "id": 27,
              "name": "LineDiscount%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 28,
              "name": "LineDiscountAmount",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 29,
              "name": "Amount",
              "type": "Decimal",
              "value": 1943.4,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 2060.0,
              "System": true
            },
            {
              "id": 74,
              "name": "GenBusPostingGroup",
              "type": "Code",
              "value": "DOMESTIC",
              "System": true
            },
            {
              "id": 75,
              "name": "GenProdPostingGroup",
              "type": "Code",
              "value": "RETAIL",
              "System": true
            },
            {
              "id": 89,
              "name": "VATBusPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 90,
              "name": "VATProdPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5402,
              "name": "VariantCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5403,
              "name": "BinCode",
              "type": "Code",
              "value": null,
              "System": true
            }
          ]
        },
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "Adventure",
          "position": "Document No.=CONST(PS-INV103197),Line No.=CONST(20000)",
          "recordId": "Sales Invoice Line: PS-INV103197,20000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103197",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 20000,
                "System": true
              }
            ]
          },
          "fieldCount": 20,
          "fields": [
            {
              "id": 3,
              "name": "DocumentNo",
              "type": "Code",
              "value": "PS-INV103197",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 20000,
              "System": true
            },
            {
              "id": 5,
              "name": "Type",
              "type": "Option",
              "value": "Item",
              "System": true
            },
            {
              "id": 6,
              "name": "No",
              "type": "Code",
              "value": "1988-S",
              "System": true
            },
            {
              "id": 7,
              "name": "LocationCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 11,
              "name": "Description",
              "type": "Text",
              "value": "SEOUL Guest Chair, red",
              "System": true
            },
            {
              "id": 13,
              "name": "UnitofMeasure",
              "type": "Text",
              "value": "Piece",
              "System": true
            },
            {
              "id": 15,
              "name": "Quantity",
              "type": "Decimal",
              "value": 5.0,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 25,
              "name": "VAT%",
              "type": "Decimal",
              "value": 6.0,
              "System": true
            },
            {
              "id": 27,
              "name": "LineDiscount%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 28,
              "name": "LineDiscountAmount",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 29,
              "name": "Amount",
              "type": "Decimal",
              "value": 964.0,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 1021.84,
              "System": true
            },
            {
              "id": 74,
              "name": "GenBusPostingGroup",
              "type": "Code",
              "value": "DOMESTIC",
              "System": true
            },
            {
              "id": 75,
              "name": "GenProdPostingGroup",
              "type": "Code",
              "value": "RETAIL",
              "System": true
            },
            {
              "id": 89,
              "name": "VATBusPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 90,
              "name": "VATProdPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5402,
              "name": "VariantCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5403,
              "name": "BinCode",
              "type": "Code",
              "value": null,
              "System": true
            }
          ]
        }
      ]
    },
    {
      "id": 112,
      "name": "SalesInvoiceHeader",
      "company": "Adventure",
      "position": "No.=CONST(PS-INV103223)",
      "recordId": "Sales Invoice Header: PS-INV103223",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103223",
            "System": true
          }
        ]
      },
      "fieldCount": 15,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103223",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "50000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Relecloud",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-04-10",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-04-24",
          "System": true
        },
        {
          "id": 28,
          "name": "LocationCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 32,
          "name": "CurrencyCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 44,
          "name": "OrderNo",
          "type": "Code",
          "value": "S-ORD101014",
          "System": true
        },
        {
          "id": 53,
          "name": "AppliestoDocNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 60,
          "name": "Amount",
          "type": "Decimal",
          "value": 4336.0,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 4596.16,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "25 Water Way",
          "System": true
        },
        {
          "id": 83,
          "name": "SelltoCity",
          "type": "Text",
          "value": "Atlanta",
          "System": true
        },
        {
          "id": 111,
          "name": "PreAssignedNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 1303,
          "name": "RemainingAmount",
          "type": "Decimal",
          "value": 4596.16,
          "System": false
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "Adventure",
          "position": "Document No.=CONST(PS-INV103223),Line No.=CONST(10000)",
          "recordId": "Sales Invoice Line: PS-INV103223,10000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103223",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 10000,
                "System": true
              }
            ]
          },
          "fieldCount": 20,
          "fields": [
            {
              "id": 3,
              "name": "DocumentNo",
              "type": "Code",
              "value": "PS-INV103223",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 10000,
              "System": true
            },
            {
              "id": 5,
              "name": "Type",
              "type": "Option",
              "value": "Item",
              "System": true
            },
            {
              "id": 6,
              "name": "No",
              "type": "Code",
              "value": "1906-S",
              "System": true
            },
            {
              "id": 7,
              "name": "LocationCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 11,
              "name": "Description",
              "type": "Text",
              "value": "ATHENS Mobile Pedestal",
              "System": true
            },
            {
              "id": 13,
              "name": "UnitofMeasure",
              "type": "Text",
              "value": "Piece",
              "System": true
            },
            {
              "id": 15,
              "name": "Quantity",
              "type": "Decimal",
              "value": 10.0,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 433.6,
              "System": true
            },
            {
              "id": 25,
              "name": "VAT%",
              "type": "Decimal",
              "value": 6.0,
              "System": true
            },
            {
              "id": 27,
              "name": "LineDiscount%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 28,
              "name": "LineDiscountAmount",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 29,
              "name": "Amount",
              "type": "Decimal",
              "value": 4336.0,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 4596.16,
              "System": true
            },
            {
              "id": 74,
              "name": "GenBusPostingGroup",
              "type": "Code",
              "value": "DOMESTIC",
              "System": true
            },
            {
              "id": 75,
              "name": "GenProdPostingGroup",
              "type": "Code",
              "value": "RETAIL",
              "System": true
            },
            {
              "id": 89,
              "name": "VATBusPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 90,
              "name": "VATProdPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5402,
              "name": "VariantCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5403,
              "name": "BinCode",
              "type": "Code",
              "value": null,
              "System": true
            }
          ]
        }
      ]
    },
    {
      "id": 112,
      "name": "SalesInvoiceHeader",
      "company": "Adventure",
      "position": "No.=CONST(PS-INV103285)",
      "recordId": "Sales Invoice Header: PS-INV103285",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103285",
            "System": true
          }
        ]
      },
      "fieldCount": 15,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103285",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "20000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Trey Research",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2024-04-09",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2024-04-23",
          "System": true
        },
        {
          "id": 28,
          "name": "LocationCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 32,
          "name": "CurrencyCode",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 44,
          "name": "OrderNo",
          "type": "Code",
          "value": "S-ORD101173",
          "System": true
        },
        {
          "id": 53,
          "name": "AppliestoDocNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 60,
          "name": "Amount",
          "type": "Decimal",
          "value": 192.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 192.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "153 Thomas Drive",
          "System": true
        },
        {
          "id": 83,
          "name": "SelltoCity",
          "type": "Text",
          "value": "Chicago",
          "System": true
        },
        {
          "id": 111,
          "name": "PreAssignedNo",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 1303,
          "name": "RemainingAmount",
          "type": "Decimal",
          "value": 192.8,
          "System": false
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "Adventure",
          "position": "Document No.=CONST(PS-INV103285),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103285,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103285",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 1000,
                "System": true
              }
            ]
          },
          "fieldCount": 20,
          "fields": [
            {
              "id": 3,
              "name": "DocumentNo",
              "type": "Code",
              "value": "PS-INV103285",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 1000,
              "System": true
            },
            {
              "id": 5,
              "name": "Type",
              "type": "Option",
              "value": "Item",
              "System": true
            },
            {
              "id": 6,
              "name": "No",
              "type": "Code",
              "value": "1900-S",
              "System": true
            },
            {
              "id": 7,
              "name": "LocationCode",
              "type": "Code",
              "value": "EAST",
              "System": true
            },
            {
              "id": 11,
              "name": "Description",
              "type": "Text",
              "value": "PARIS Guest Chair, black",
              "System": true
            },
            {
              "id": 13,
              "name": "UnitofMeasure",
              "type": "Text",
              "value": "Piece",
              "System": true
            },
            {
              "id": 15,
              "name": "Quantity",
              "type": "Decimal",
              "value": 1.0,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 25,
              "name": "VAT%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 27,
              "name": "LineDiscount%",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 28,
              "name": "LineDiscountAmount",
              "type": "Decimal",
              "value": null,
              "System": true
            },
            {
              "id": 29,
              "name": "Amount",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 192.8,
              "System": true
            },
            {
              "id": 74,
              "name": "GenBusPostingGroup",
              "type": "Code",
              "value": "DOMESTIC",
              "System": true
            },
            {
              "id": 75,
              "name": "GenProdPostingGroup",
              "type": "Code",
              "value": "RETAIL",
              "System": true
            },
            {
              "id": 89,
              "name": "VATBusPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 90,
              "name": "VATProdPostingGroup",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5402,
              "name": "VariantCode",
              "type": "Code",
              "value": null,
              "System": true
            },
            {
              "id": 5403,
              "name": "BinCode",
              "type": "Code",
              "value": null,
              "System": true
            }
          ]
        }
      ]
    }
  ]
}
```
