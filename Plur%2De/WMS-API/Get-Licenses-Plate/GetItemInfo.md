**ProcessMethod**: GetItemInfo

**Description**:
This method returns the history of a specific License Plate..

**Input**:
**Parameters**: Status of the LP, the options are of the integer type as seen below
-	**No**: License Plate Number.

**Ouput**: 
-	**LicensePlateEntries**:The output is an array that contains all the history of transactions, amount changes, bins, of a LP.

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

![image.png](/.attachments/image-383553e4-0404-4c82-afcf-613728dd266c.png)

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


