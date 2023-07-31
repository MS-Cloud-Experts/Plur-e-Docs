**ProcessMethod**: GetCustomers

**Description**:

Method to fetch customers that are associated with a SalesPerson

**Ouput**: 
- **Customers:** Fetches the list of customers filtered by the assigned SalesPerson


**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"GetCustomers\",\"Parameters\":[{\"pageSize\":\"0\",\"position\":\"\",\"salesPerson\":\"BC\"}]}"`

Outputs:

```
{
  "Customers": [
    {
      "id": 18,
      "name": "Customer",
      "company": "CRONUS USA, Inc.",
      "position": "No.=CONST(10000)",
      "recordId": "Customer: 10000",
      "primaryKey": {
        "fieldCount": 1,
        "fields": [
          {
            "id": 1,
            "name": "No",
            "type": "Code",
            "value": "10000",
            "System": true
          }
        ]
      },
      "fieldCount": 53,
      "fields": [
        {
          "id": 0,
          "name": "timestamp",
          "type": "BigInteger",
          "value": 3332759,
          "System": true
        },
        {
          "id": 1,
          "name": "No",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 2,
          "name": "Name",
          "type": "Text",
          "value": "Adatum Corporation",
          "System": true
        },
        {
          "id": 3,
          "name": "SearchName",
          "type": "Code",
          "value": "ADATUM CORPORATION",
          "System": true
        },
        {
          "id": 4,
          "name": "Name2",
          "type": "Text",
          "value": null,
          "System": true
        },
        {
          "id": 5,
          "name": "Address",
          "type": "Text",
          "value": "192 Market Square",
          "System": true
        },
        {
          "id": 6,
          "name": "Address2",
          "type": "Text",
          "value": null,
          "System": true
        },
        {
          "id": 7,
          "name": "City",
          "type": "Text",
          "value": "Atlanta",
          "System": true
        },
        {
          "id": 8,
          "name": "Contact",
          "type": "Text",
          "value": "Robert Townes",
          "System": true
        },
        {
          "id": 9,
          "name": "PhoneNo",
          "type": "Text",
          "value": null,
          "System": true
        },
        {
          "id": 10,
          "name": "TelexNo",
          "type": "Text",
          "value": null,
          "System": true
        },
        {
          "id": 11,
          "name": "DocumentSendingProfile",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 14,
          "name": "OurAccountNo",
          "type": "Text",
          "value": null,
          "System": true
        },
        {
          "id": 15,
          "name": "TerritoryCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 16,
          "name": "GlobalDimension1Code",
          "type": "Code",
          "value": "SALES",
          "System": true
        },
        {
          "id": 17,
          "name": "GlobalDimension2Code",
          "type": "Code",
          "value": "SMALL",
          "System": true
        },
        {
          "id": 18,
          "name": "ChainName",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 19,
          "name": "BudgetedAmount",
          "type": "Decimal",
          "value": null,
          "System": true
        },
        {
          "id": 20,
          "name": "CreditLimitLCY",
          "type": "Decimal",
          "value": null,
          "System": true
        },
        {
          "id": 21,
          "name": "CustomerPostingGroup",
          "type": "Code",
          "value": "DOMESTIC",
          "System": true
        },
        {
          "id": 22,
          "name": "CurrencyCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 23,
          "name": "CustomerPriceGroup",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 24,
          "name": "LanguageCode",
          "type": "Code",
          "value": "ENU",
          "System": true
        },
        {
          "id": 26,
          "name": "StatisticsGroup",
          "type": "Integer",
          "value": null,
          "System": true
        },
        {
          "id": 27,
          "name": "PaymentTermsCode",
          "type": "Code",
          "value": "1M(8D)",
          "System": true
        },
        {
          "id": 28,
          "name": "FinChargeTermsCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 29,
          "name": "SalespersonCode",
          "type": "Code",
          "value": "BC",
          "System": true
        },
        {
          "id": 30,
          "name": "ShipmentMethodCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 31,
          "name": "ShippingAgentCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 32,
          "name": "PlaceofExport",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 33,
          "name": "InvoiceDiscCode",
          "type": "Code",
          "value": "10000",
          "System": true
        },
        {
          "id": 34,
          "name": "CustomerDiscGroup",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 35,
          "name": "CountryRegionCode",
          "type": "Code",
          "value": "US",
          "System": true
        },
        {
          "id": 36,
          "name": "CollectionMethod",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 37,
          "name": "Amount",
          "type": "Decimal",
          "value": null,
          "System": true
        },
        {
          "id": 46,
          "name": "Priority",
          "type": "Integer",
          "value": null,
          "System": true
        },
        {
          "id": 53,
          "name": "LastModifiedDateTime",
          "type": "DateTime",
          "value": "2023-06-06T21:07:48.9870000Z",
          "System": true
        },
        {
          "id": 54,
          "name": "LastDateModified",
          "type": "Date",
          "value": "2023-06-06",
          "System": true
        },
        {
          "id": 62,
          "name": "SalesLCY",
          "type": "Decimal",
          "value": 251663.7,
          "System": true
        },
        {
          "id": 66,
          "name": "BalanceDue",
          "type": "Decimal",
          "value": 28305.49,
          "System": true
        },
        {
          "id": 72,
          "name": "FinanceChargeMemoAmounts",
          "type": "Decimal",
          "value": null,
          "System": true
        },
        {
          "id": 74,
          "name": "PaymentsLCY",
          "type": "Decimal",
          "value": 232466.11,
          "System": true
        },
        {
          "id": 80,
          "name": "ApplicationMethod",
          "type": "Option",
          "value": "Manual",
          "System": true
        },
        {
          "id": 83,
          "name": "LocationCode",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 88,
          "name": "GenBusPostingGroup",
          "type": "Code",
          "value": "DOMESTIC",
          "System": true
        },
        {
          "id": 90,
          "name": "GLN",
          "type": "Code",
          "value": null,
          "System": true
        },
        {
          "id": 91,
          "name": "PostCode",
          "type": "Code",
          "value": "31772",
          "System": true
        },
        {
          "id": 92,
          "name": "County",
          "type": "Text",
          "value": "GA",
          "System": true
        },
        {
          "id": 97,
          "name": "DebitAmount",
          "type": "Decimal",
          "value": 273686.46,
          "System": true
        },
        {
          "id": 98,
          "name": "CreditAmount",
          "type": "Decimal",
          "value": 245380.97,
          "System": true
        },
        {
          "id": 100,
          "name": "CreditAmountLCY",
          "type": "Decimal",
          "value": 245380.97,
          "System": true
        },
        {
          "id": 102,
          "name": "EMail",
          "type": "Text",
          "value": "robert.townes@contoso.com",
          "System": true
        },
        {
          "id": 110,
          "name": "VATBusPostingGroup",
          "type": "Code",
          "value": null,
          "System": true
        }
      ],
      "ShipToAddress": [
        {
          "id": 222,
          "name": "ShiptoAddress",
          "company": "CRONUS USA, Inc.",
          "position": "Customer No.=CONST(10000),Code=CONST(LEWES ROAD)",
          "recordId": "Ship-to Address: 10000,LEWES ROAD",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 1,
                "name": "CustomerNo",
                "type": "Code",
                "value": "10000",
                "System": false
              },
              {
                "id": 2,
                "name": "Code",
                "type": "Code",
                "value": "LEWES ROAD",
                "System": false
              }
            ]
          },
          "fieldCount": 33,
          "fields": [
            {
              "id": 1,
              "name": "CustomerNo",
              "type": "Code",
              "value": "10000",
              "System": false
            },
            {
              "id": 2,
              "name": "Code",
              "type": "Code",
              "value": "LEWES ROAD",
              "System": false
            },
            {
              "id": 3,
              "name": "Name",
              "type": "Text",
              "value": "Adatum Corporation",
              "System": false
            },
            {
              "id": 4,
              "name": "Name2",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 5,
              "name": "Address",
              "type": "Text",
              "value": "2 Lewes Road",
              "System": false
            },
            {
              "id": 6,
              "name": "Address2",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "City",
              "type": "Text",
              "value": "Atlanta",
              "System": false
            },
            {
              "id": 8,
              "name": "Contact",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 9,
              "name": "PhoneNo",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 10,
              "name": "TelexNo",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 30,
              "name": "ShipmentMethodCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 31,
              "name": "ShippingAgentCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 32,
              "name": "PlaceofExport",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 35,
              "name": "CountryRegionCode",
              "type": "Code",
              "value": "US",
              "System": false
            },
            {
              "id": 54,
              "name": "LastDateModified",
              "type": "Date",
              "value": "2023-05-12",
              "System": false
            },
            {
              "id": 83,
              "name": "LocationCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 84,
              "name": "FaxNo",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 85,
              "name": "TelexAnswerBack",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 90,
              "name": "GLN",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 91,
              "name": "PostCode",
              "type": "Code",
              "value": "31772",
              "System": false
            },
            {
              "id": 92,
              "name": "County",
              "type": "Text",
              "value": "GA",
              "System": false
            },
            {
              "id": 102,
              "name": "EMail",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 103,
              "name": "HomePage",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 108,
              "name": "TaxAreaCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 109,
              "name": "TaxLiable",
              "type": "Boolean",
              "value": false,
              "System": false
            },
            {
              "id": 5792,
              "name": "ShippingAgentServiceCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 5900,
              "name": "ServiceZoneCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 10004,
              "name": "UPSZone",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{8DB5DE2E-078B-ED11-AAD8-000D3A21EDC2}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-01-03T01:37:36.8800000Z",
              "System": false
            },
            {
              "id": 2000000002,
              "name": "SystemCreatedBy",
              "type": "GUID",
              "value": "{00000000-0000-0000-0000-000000000001}",
              "System": false
            },
            {
              "id": 2000000003,
              "name": "SystemModifiedAt",
              "type": "DateTime",
              "value": "2023-05-12T21:03:11.4500000Z",
              "System": false
            },
            {
              "id": 2000000004,
              "name": "SystemModifiedBy",
              "type": "GUID",
              "value": "{1266B8C3-FE60-493F-B3DD-3712ED0E269F}",
              "System": false
            }
          ]
        },
        {
          "id": 222,
          "name": "ShiptoAddress",
          "company": "CRONUS USA, Inc.",
          "position": "Customer No.=CONST(10000),Code=CONST(PARK ROAD)",
          "recordId": "Ship-to Address: 10000,PARK ROAD",
          "primaryKey": {
            "fieldCount": 2,
            "fields": [
              {
                "id": 1,
                "name": "CustomerNo",
                "type": "Code",
                "value": "10000",
                "System": false
              },
              {
                "id": 2,
                "name": "Code",
                "type": "Code",
                "value": "PARK ROAD",
                "System": false
              }
            ]
          },
          "fieldCount": 33,
          "fields": [
            {
              "id": 1,
              "name": "CustomerNo",
              "type": "Code",
              "value": "10000",
              "System": false
            },
            {
              "id": 2,
              "name": "Code",
              "type": "Code",
              "value": "PARK ROAD",
              "System": false
            },
            {
              "id": 3,
              "name": "Name",
              "type": "Text",
              "value": "Adatum Corporation",
              "System": false
            },
            {
              "id": 4,
              "name": "Name2",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 5,
              "name": "Address",
              "type": "Text",
              "value": "10 Park Road",
              "System": false
            },
            {
              "id": 6,
              "name": "Address2",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 7,
              "name": "City",
              "type": "Text",
              "value": "Atlanta",
              "System": false
            },
            {
              "id": 8,
              "name": "Contact",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 9,
              "name": "PhoneNo",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 10,
              "name": "TelexNo",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 30,
              "name": "ShipmentMethodCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 31,
              "name": "ShippingAgentCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 32,
              "name": "PlaceofExport",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 35,
              "name": "CountryRegionCode",
              "type": "Code",
              "value": "US",
              "System": false
            },
            {
              "id": 54,
              "name": "LastDateModified",
              "type": "Date",
              "value": "2023-05-12",
              "System": false
            },
            {
              "id": 83,
              "name": "LocationCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 84,
              "name": "FaxNo",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 85,
              "name": "TelexAnswerBack",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 90,
              "name": "GLN",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 91,
              "name": "PostCode",
              "type": "Code",
              "value": "31772",
              "System": false
            },
            {
              "id": 92,
              "name": "County",
              "type": "Text",
              "value": "GA",
              "System": false
            },
            {
              "id": 102,
              "name": "EMail",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 103,
              "name": "HomePage",
              "type": "Text",
              "value": null,
              "System": false
            },
            {
              "id": 108,
              "name": "TaxAreaCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 109,
              "name": "TaxLiable",
              "type": "Boolean",
              "value": false,
              "System": false
            },
            {
              "id": 5792,
              "name": "ShippingAgentServiceCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 5900,
              "name": "ServiceZoneCode",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 10004,
              "name": "UPSZone",
              "type": "Code",
              "value": null,
              "System": false
            },
            {
              "id": 2000000000,
              "name": "$systemId",
              "type": "GUID",
              "value": "{8EB5DE2E-078B-ED11-AAD8-000D3A21EDC2}",
              "System": false
            },
            {
              "id": 2000000001,
              "name": "SystemCreatedAt",
              "type": "DateTime",
              "value": "2023-01-03T01:37:36.8870000Z",
              "System": false
            },
            {
              "id": 2000000002,
              "name": "SystemCreatedBy",
              "type": "GUID",
              "value": "{00000000-0000-0000-0000-000000000001}",
              "System": false
            },
            {
              "id": 2000000003,
              "name": "SystemModifiedAt",
              "type": "DateTime",
              "value": "2023-05-12T21:24:08.2600000Z",
              "System": false
            },
            {
              "id": 2000000004,
              "name": "SystemModifiedBy",
              "type": "GUID",
              "value": "{1266B8C3-FE60-493F-B3DD-3712ED0E269F}",
              "System": false
            }
          ]
        }
      ]
    }
  ]
}
```

**EXEMPTIONS**

- **Error:** SalesPerson who does not exist

```
"error": {
        "code": "Internal_RecordNotFound",
        "message": "The Salesperson/Purchaser does not exist. Identification fields and values: Code='BC2'  CorrelationId:  1822e662-966b-4153-bd3c-f9bb8bfea1bf."
    }
```


