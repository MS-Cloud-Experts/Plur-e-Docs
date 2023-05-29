**ProcessMethod**: GetLicencesPlate

**Description**:
The method that returns the combination of License Plate Headers / License Plate Lines according to the number with which it is filtered.

**Input**:
**Parameters**: 
-	**No**: Number of the License Plate that you want to filter.

**Output**: 
-	**LicensePlates**: Contains the information of a License Plate header in **LicensePlatesHeaders** and **LicensePlatesLines** contains an array of License Plate Lines.
-	
**Example**:

Request:

```
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP000205"
    }
  ]
}
```



Outputs:

![image.png](/.attachments/image-5195c8c8-5405-4be5-8581-fd9d0f152dc0.png)

```
{
  "LicensePlates": [
    {
      "LPDocumentNo": "LP-00161",
      "LPDocumentType": "Pallet",
      "PLULicensePlateStatus": "Stored",
      "ParentLPNo": "",
      "LocationCode": "NEWWMS",
      "BinCode": "FLOOR",
      "WhseDocumentNo": "REG PUTAWAY-00024",
      "LPTotalQuantities": 0.0,
      "LPLines": [
        {
          "LPDocumentNo": "LP-00157",
          "LPDocumentType": "Single",
          "PLULicensePlateStatus": "Stored",
          "ParentLPNo": "LP-00161",
          "LocationCode": "NEWWMS",
          "BinCode": "FLOOR",
          "WhseDocumentNo": "REG PUTAWAY-00024",
          "LPTotalQuantities": 0.0,
          "LPLines": [
            {
              "LPDocumentNo": "LP-00157",
              "LPDocumentType": "Single",
              "LineNo": "1000",
              "No": "70063",
              "Description": "",
              "VariantCode": "RED",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            },
            {
              "LPDocumentNo": "LP-00157",
              "LPDocumentType": "Single",
              "LineNo": "2000",
              "No": "70063",
              "Description": "",
              "VariantCode": "RED",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            }
          ]
        },
        {
          "LPDocumentNo": "LP-00158",
          "LPDocumentType": "Single",
          "PLULicensePlateStatus": "Stored",
          "ParentLPNo": "LP-00161",
          "LocationCode": "NEWWMS",
          "BinCode": "FLOOR",
          "WhseDocumentNo": "REG PUTAWAY-00024",
          "LPTotalQuantities": 0.0,
          "LPLines": [
            {
              "LPDocumentNo": "LP-00158",
              "LPDocumentType": "Single",
              "LineNo": "1000",
              "No": "70063",
              "Description": "",
              "VariantCode": "YELLOW",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            },
            {
              "LPDocumentNo": "LP-00158",
              "LPDocumentType": "Single",
              "LineNo": "2000",
              "No": "70063",
              "Description": "",
              "VariantCode": "YELLOW",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            }
          ]
        },
        {
          "LPDocumentNo": "LP-00159",
          "LPDocumentType": "Single",
          "PLULicensePlateStatus": "Stored",
          "ParentLPNo": "LP-00161",
          "LocationCode": "NEWWMS",
          "BinCode": "FLOOR",
          "WhseDocumentNo": "REG PUTAWAY-00024",
          "LPTotalQuantities": 0.0,
          "LPLines": [
            {
              "LPDocumentNo": "LP-00159",
              "LPDocumentType": "Single",
              "LineNo": "1000",
              "No": "70063",
              "Description": "",
              "VariantCode": "RED",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            },
            {
              "LPDocumentNo": "LP-00159",
              "LPDocumentType": "Single",
              "LineNo": "2000",
              "No": "70063",
              "Description": "",
              "VariantCode": "RED",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            }
          ]
        },
        {
          "LPDocumentNo": "LP-00160",
          "LPDocumentType": "Single",
          "PLULicensePlateStatus": "Stored",
          "ParentLPNo": "LP-00161",
          "LocationCode": "NEWWMS",
          "BinCode": "FLOOR",
          "WhseDocumentNo": "REG PUTAWAY-00024",
          "LPTotalQuantities": 0.0,
          "LPLines": [
            {
              "LPDocumentNo": "LP-00160",
              "LPDocumentType": "Single",
              "LineNo": "1000",
              "No": "70063",
              "Description": "",
              "VariantCode": "YELLOW",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            },
            {
              "LPDocumentNo": "LP-00160",
              "LPDocumentType": "Single",
              "LineNo": "2000",
              "No": "70063",
              "Description": "",
              "VariantCode": "YELLOW",
              "LotNo": "",
              "ExpirationDate": "05/25/23"
            }
          ]
        }
      ]
    }
  ]
}
```
**Error**:
```
{
  "Error": {
    "Code": "Not found",
    "Message": "The Licences Plate List is Empty"
  }
}
```


