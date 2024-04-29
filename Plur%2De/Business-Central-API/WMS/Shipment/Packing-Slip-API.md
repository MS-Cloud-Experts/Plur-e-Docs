**ProcessMethods**: 

GetPackingSlip


**Parameters**: 

-	**DocumentNo**: Warehouse Pick No.



**Example Request**:

```
"jsonRequest":"{\"ProcessMethod\":\"GetPackingSlip\",\"Parameters\":[{\"DocumentNo\":\"WHSE PICK-00019\"}]}"
```

**Output GetWHSPickInShipments**
```
{
  "CompanyInfo": {
    "Name": "Adventure",
    "Address": "7122 South Ashford Street",
    "Address2": "Westminster",
    "City": "Atlanta",
    "ZipCode": "31772",
    "PhoneNo": "+1 425 555 0100",
    "Email": ""
  },
  "ShipTo": {
    "Name": "Adatum Corporation",
    "Company": "Adventure",
    "Address1": "192 Market Square",
    "Address2": "",
    "City": "Atlanta",
    "State": "GA",
    "Country": "US",
    "PostalCode": "31772",
    "Phone": ""
  },
  "BillTo": {
    "Name": "Adatum Corporation",
    "Company": "Adventure",
    "Address1": "192 Market Square",
    "Address2": "",
    "City": "Atlanta",
    "State": "GA",
    "Country": "US",
    "PostalCode": "31772",
    "Phone": ""
  },
  "CustomerUsername": "",
  "PickingDate": "0001-01-01",
  "CustPO#": "",
  "ShipVia": "seko_ltl_walleted",
  "PaymentTerm": {
    "PaymentTermsCode": "1M(8D)",
    "PaymentMethodCode": ""
  },
  "ProcessBy": "DARIO.SANCHEZ",
  "WarehousePickLines": [
    {
      "No": "WHSE PICK-00019",
      "LineNo": 10000,
      "ItemNo": "1896-S",
      "VariantCode": "",
      "Description": "ATHENS Desk",
      "Qty": 2.0,
      "SourceNo": "S-ORD101034",
      "LocationCode": "NEWWMS",
      "BinCode": "STO-4",
      "PackageInfo": [
        {
          "PackageNo": 1,
          "LineNo": 1000,
          "SourceNo": "S-ORD101034",
          "SourceLineNo": 10000,
          "WarehouseDocumentNo": "WHSE PICK-00019",
          "WarehouseLineNo": 10000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "SerialNo": "",
          "LotNo": "",
          "ItemPrice": 1000.8,
          "QtyToHandle": 2
        }
      ]
    },
    {
      "No": "WHSE PICK-00019",
      "LineNo": 30000,
      "ItemNo": "1900-S",
      "VariantCode": "",
      "Description": "PARIS Guest Chair, black",
      "Qty": 2.0,
      "SourceNo": "S-ORD101035",
      "LocationCode": "NEWWMS",
      "BinCode": "STO-3",
      "PackageInfo": [
        {
          "PackageNo": 1,
          "LineNo": 2000,
          "SourceNo": "S-ORD101035",
          "SourceLineNo": 10000,
          "WarehouseDocumentNo": "WHSE PICK-00019",
          "WarehouseLineNo": 30000,
          "ItemNo": "1900-S",
          "VariantCode": "",
          "SerialNo": "",
          "LotNo": "",
          "ItemPrice": 192.8,
          "QtyToHandle": 2
        }
      ]
    }
  ]
}

```
