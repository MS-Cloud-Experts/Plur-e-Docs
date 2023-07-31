**ProcessMethod**: PostedSalesInvoices

**Description**:
Method that brings Posted Sales Invoice filtered by the SalesPerson

**Ouput**: 
-	**Posted Sales Invoice:** JsonArray with Posted Sales Invoice assigned to a SalesPerson

**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"PostedSalesInvoices\",\"Parameters\":[{\"paid\":true,\"salesPerson\":\"BC\"}]}"`

**Outputs:**

```
{
  "SalesOrders": [
    {
      "id": 112,
      "name": "SalesInvoiceHeader",
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103216)",
      "recordId": "Sales Invoice Header: PS-INV103216",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103216",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103216",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
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
          "value": "2023-05-10",
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
          "value": "S-ORD101006",
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
          "value": 12009.6,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 12009.6,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103216),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103216,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103216",
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
              "value": "PS-INV103216",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 12.0,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 1000.8,
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
              "value": 12009.6,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 12009.6,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103217)",
      "recordId": "Sales Invoice Header: PS-INV103217",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103217",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103217",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-04-27",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-05-27",
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
          "value": "S-ORD101008",
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
          "value": 190.1,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 190.1,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103217),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103217,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103217",
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
              "value": "PS-INV103217",
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
              "value": "1972-S",
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
              "value": "MUNICH Swivel Chair, yellow",
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
              "value": 190.1,
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
              "value": 190.1,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 190.1,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103218)",
      "recordId": "Sales Invoice Header: PS-INV103218",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103218",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103218",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-04",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-04",
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
          "value": "S-ORD101016",
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
          "value": 578.4,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 578.4,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103218),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103218,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103218",
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
              "value": "PS-INV103218",
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
              "value": null,
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
              "value": 3.0,
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
              "value": 578.4,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 578.4,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103219)",
      "recordId": "Sales Invoice Header: PS-INV103219",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103219",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103219",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-04",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-04",
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
          "value": "S-ORD101017",
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
          "value": 578.4,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 578.4,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103219),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103219,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103219",
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
              "value": "PS-INV103219",
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
              "value": null,
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
              "value": 3.0,
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
              "value": 578.4,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 578.4,
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
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103219),Line No.=CONST(2000)",
          "recordId": "Sales Invoice Line: PS-INV103219,2000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103219",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 2000,
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
              "value": "PS-INV103219",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 2000,
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": null,
              "System": true
            },
            {
              "id": 22,
              "name": "UnitPrice",
              "type": "Decimal",
              "value": 1000.8,
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
              "value": null,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": null,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103220)",
      "recordId": "Sales Invoice Header: PS-INV103220",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103220",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103220",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-08",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-08",
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
          "value": "S-ORD101020",
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
          "value": 771.2,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 771.2,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103220),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103220,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103220",
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
              "value": "PS-INV103220",
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
              "value": null,
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
              "value": 2.0,
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
              "value": 385.6,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 385.6,
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
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103220),Line No.=CONST(2000)",
          "recordId": "Sales Invoice Line: PS-INV103220,2000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103220",
                "System": true
              },
              {
                "id": 4,
                "name": "LineNo",
                "type": "Integer",
                "value": 2000,
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
              "value": "PS-INV103220",
              "System": true
            },
            {
              "id": 4,
              "name": "LineNo",
              "type": "Integer",
              "value": 2000,
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
              "value": null,
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
              "value": 2.0,
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
              "value": 385.6,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 385.6,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103221)",
      "recordId": "Sales Invoice Header: PS-INV103221",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103221",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103221",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-09",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-09",
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
          "value": "S-ORD101022",
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
          "value": 771.2,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 771.2,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103221),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103221,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103221",
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
              "value": "PS-INV103221",
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
              "value": null,
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
              "value": 4.0,
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
              "value": 771.2,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 771.2,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103222)",
      "recordId": "Sales Invoice Header: PS-INV103222",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103222",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103222",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-09",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-09",
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
          "value": "S-ORD101022",
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
          "value": 1156.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 1156.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103222),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103222,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103222",
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
              "value": "PS-INV103222",
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
              "value": null,
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
              "value": 6.0,
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
              "value": 1156.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 1156.8,
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
      "company": "CRONUS USA, Inc.",
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
      "fieldCount": 14,
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
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-16",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-16",
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
          "value": "S-ORD101024",
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
          "value": 3002.4,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 3002.4,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103223),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103223,1000",
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
              "value": "PS-INV103223",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 1000.8,
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
              "value": 3002.4,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 3002.4,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103224)",
      "recordId": "Sales Invoice Header: PS-INV103224",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103224",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103224",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-23",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-23",
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
          "value": 1000.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 1000.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
          "value": "S-INV102225",
          "System": true
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103224),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103224,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103224",
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
              "value": "PS-INV103224",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 1000.8,
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
              "value": 1000.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 1000.8,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103225)",
      "recordId": "Sales Invoice Header: PS-INV103225",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103225",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103225",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-19",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-19",
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
          "value": "S-ORD101027",
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
          "value": 3002.4,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 3002.4,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103225),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103225,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103225",
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
              "value": "PS-INV103225",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 1000.8,
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
              "value": 3002.4,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 3002.4,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103226)",
      "recordId": "Sales Invoice Header: PS-INV103226",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103226",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103226",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-30",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-30",
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
          "value": 1000.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 1000.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
          "value": "S-INV102226",
          "System": true
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103226),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103226,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103226",
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
              "value": "PS-INV103226",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 1000.8,
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
              "value": 1000.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 1000.8,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103227)",
      "recordId": "Sales Invoice Header: PS-INV103227",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103227",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103227",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-31",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-30",
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
          "value": 1000.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 1000.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
          "value": "S-INV102227",
          "System": true
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103227),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103227,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103227",
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
              "value": "PS-INV103227",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 1000.8,
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
              "value": 1000.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 1000.8,
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
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(PS-INV103228)",
      "recordId": "Sales Invoice Header: PS-INV103228",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 3,
            "name": "No",
            "type": "Code",
            "value": "PS-INV103228",
            "System": true
          }
        ]
      },
      "fieldCount": 14,
      "fields": [
        {
          "id": 3,
          "name": "No",
          "type": "Code",
          "value": "PS-INV103228",
          "System": true
        },
        {
          "id": 4,
          "name": "BilltoCustomerNo",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 5,
          "name": "BilltoName",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 20,
          "name": "PostingDate",
          "type": "Date",
          "value": "2023-05-31",
          "System": true
        },
        {
          "id": 24,
          "name": "DueDate",
          "type": "Date",
          "value": "2023-06-30",
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
          "value": 1000.8,
          "System": true
        },
        {
          "id": 61,
          "name": "AmountIncludingVAT",
          "type": "Decimal",
          "value": 1000.8,
          "System": true
        },
        {
          "id": 81,
          "name": "SelltoAddress",
          "type": "Text",
          "value": "192 Market Square",
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
          "value": "S-INV102228",
          "System": true
        }
      ],
      "OriginalPmtDiscPossible": 0,
      "SalesLines": [
        {
          "id": 113,
          "name": "SalesInvoiceLine",
          "company": "CRONUS USA, Inc.",
          "position": "Document No.=CONST(PS-INV103228),Line No.=CONST(1000)",
          "recordId": "Sales Invoice Line: PS-INV103228,1000",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 3,
                "name": "DocumentNo",
                "type": "Code",
                "value": "PS-INV103228",
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
              "value": "PS-INV103228",
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
              "value": "1896-S",
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
              "value": "ATHENS Desk",
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
              "value": 1000.8,
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
              "value": 1000.8,
              "System": true
            },
            {
              "id": 30,
              "name": "AmountIncludingVAT",
              "type": "Decimal",
              "value": 1000.8,
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


