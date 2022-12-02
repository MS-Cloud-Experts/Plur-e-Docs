**ProcessMethod**: GetDefaultBin

**Description**:
This method returns the Default Bin used to edit a Put-Away

**Parameters**: 

**Ouput**: Returns list of Bins available to be adjusted in the License Plate
-	**Bins**: is a Json array that contains the Bin Code and Location code to which each possible assignable BIN belongs.

**Example**:

```
**Request:**
{
  "ProcessMethod": "GetPossiblesBinFromPutAway",
  "Parameters": [
    {
      "No": "LP-00060"
    }
  ]
}
```

**Output**:

**WarehouseReceipts:**

![image.png](/.attachments/image-8c85a697-b947-4caa-b2f7-24d30ec20db0.png)

**Output:**

```
{
  "Bins": [
    {
      "BinCode": "REC-1",
      "LocationCode": "WMS"
    },
    {
      "BinCode": "REC-2",
      "LocationCode": "WMS"
    }
  ]
}
```

**Error**:

```
{
  "Error": {
    "Code": "Not Found",
    "Message": "The Licences Plate does not exist"
  }
}
```
