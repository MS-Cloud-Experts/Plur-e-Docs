**ProcessMethod**: Get_LPLedgerEntries

**Description**:
Method that returns the combination of Registration Headers / Registration Lines according to the number of the **Warehouse Receipt** with which it is filtered.

**Input**:
**Parameters**: Status of the LP, the options are of the integer type as seen below
-	**No**: Warehouse Receipt Number.
-	**IsPallet**: if the variable is true it indicates that it is Pallet, otherwise it is Single.
-	**LicensePlateStatus**:  

 -value(0; "Pre-Labeled") 
 -value(1; "Received") -> Warehouse Receipt
 -value(2; "Labeled") -> Warehouse PutAway
 -value(3; "Stored") -> Warehouse Registered PutAway
 -value(4; "Piked") 
 -value(5; "Packed") 
 -value(6; "Released") 
 -value(7; "Voided")
 -value(8; "Process") 

**Ouput**: 
-	**LicensePlates**: Contains the information of a License Plate header in **LicensePlatesHeaders** and **LicensePlatesLines** contains an array of License Plate Lines.
-	
**Example**:

Request:

```
{
  "ProcessMethod": "Get_LPLedgerEntries",
  "Parameters": [
    {
      "No": "LP-0000779"
    }
  ]
}
```



Outputs:

![image.png](/.attachments/image-5195c8c8-5405-4be5-8581-fd9d0f152dc0.png)

```
{
  "LicensePlateEntries": [
    {
      "EntryType": "Created",
      "LicensePlateStatus": "Received",
      "Document": "Warehouse Receipt",
      "DocumentNo": "WHSE REC-0000026",
      "LocationCode": "WMS",
      "BinCode": "REC-01",
      "Quantity": "0",
      "UnitofMeasure": "",
      "PostingDate": "2022-10-07T21:44:42.6930000Z",
      "UserName": "INTEGRATION WITH PLUR-E APP"
    },
    {
      "EntryType": "Modified",
      "LicensePlateStatus": "Received",
      "Document": "Warehouse Receipt",
      "DocumentNo": "WHSE REC-0000026",
      "LocationCode": "WMS",
      "BinCode": "REC-01",
      "Quantity": "1",
      "UnitofMeasure": "PCS",
      "PostingDate": "2022-10-07T21:44:42.7070000Z",
      "UserName": "INTEGRATION WITH PLUR-E APP"
    },
    {
      "EntryType": "Modified",
      "LicensePlateStatus": "Received",
      "Document": "Warehouse Receipt",
      "DocumentNo": "WHSE REC-0000026",
      "LocationCode": "WMS",
      "BinCode": "REC-01",
      "Quantity": "1",
      "UnitofMeasure": "PCS",
      "PostingDate": "2022-10-07T21:46:17.7800000Z",
      "UserName": "INTEGRATION WITH PLUR-E APP"
    },
    {
      "EntryType": "Modified",
      "LicensePlateStatus": "Labeled",
      "Document": "Warehouse Putway",
      "DocumentNo": "WHSE PUTAWAY-0000072",
      "LocationCode": "WMS",
      "BinCode": "REC-01",
      "Quantity": "1",
      "UnitofMeasure": "PCS",
      "PostingDate": "2022-10-07T21:46:18.3100000Z",
      "UserName": "INTEGRATION WITH PLUR-E APP"
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


