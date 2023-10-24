**Item Tracking Lines Open:**

![image.png](/.attachments/image-723d75d5-d765-4c0c-8e3c-f6362c9721ff.png)

**Item Tracking:**

![image.png](/.attachments/image-5918d26f-6798-47ce-ab89-1fa604a2f02a.png)

![image.png](/.attachments/image-45d7e8d5-1bc4-4bf7-9b3a-571922e61f0b.png)

**Input**

```
  "ProcessMethod": "GetItemTrackingSpecificationNewSimple",
  "Parameters": [
    {
      "SourceType": 39,
      "SourceSubtype": 1,
      "SourceNo": "PO-109960",
      "SourceRefNo": 10000
    }
  ]
}
```

**SourceNo**
- Sales Documents: 
SourceNo:= Sales Order No.
- Purch Documents: 
SourceNo:= Purch Order No.
- Warehouse Receipts
SourceNo: Warehouse Receipt Lines.SourceNo

**SourceRefNo**
- Sales Documents: 
SourceRefNo:= Sales Order Line No.
- Purch Documents: 
SourceRefNo:= Purch Order Line No.
- Warehouse Receipts
SourceRefNo: Warehouse Receipt Lines.SourceLineNo

**SourceType:** 
- Sales Documents: 
SourceType := 37
- Purch Documents: 
SourceType := 39
- Warehouse Receipts
SourceType : Warehouse Receipt Lines.SourceType

**SourceSubtype:** 
- Sales Documents: 
SourceSubtype:= 0
- Purch Documents: 
SourceSubtype:= 0
- Warehouse Receipts
SourceSubtype: Warehouse Receipt Lines.SourceSubtype

**OutPut**

```
{
  "TrackingSpecificationOpen": [
    {
      "ItemNo": "K2FWVSWNG",
      "LocationCode": "ASIA",
      "SerialNo": "HOLADARIO",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    },
    {
      "ItemNo": "K2FWVSWNG",
      "LocationCode": "ASIA",
      "SerialNo": "SERIAL1",
      "LotNo": "",
      "ExpirationDate": "0001-01-01"
    }
  ]
}
```



**Errors**

```
{
  "Error": "The TrackingSpecification does not exist.",
  "ItemIdentifier": [
    {
      "Code": "",
      "VariantCode": "",
      "UnitofMeasureCode": ""
    }
  ]
}
```
