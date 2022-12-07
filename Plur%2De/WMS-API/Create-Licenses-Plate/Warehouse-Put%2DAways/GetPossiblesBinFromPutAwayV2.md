**ProcessMethod**: GetPossiblesBinFromPutAwayV2

**Description**:
Bring all the Bin codes available Warehouse Put Away No.

**Parameters**: 

**Input**:

**Parameters**: 
-	**No**: Warehouse Put Away No.

**Ouput**: Returns list of Bins available.
-	**Bins**: is a Json array that contains the Bin Code and Location code to which each possible assignable BIN belongs.

**Example**:

```
**Request:**
{
  "ProcessMethod": "GetPossiblesBinFromPutAwayV2",
  "Parameters": [
    {
      "No": "WHSE PUTAWAY-00001"
    }
  ]
}
```

**Output**:

**WarehousePutaways:**

![image.png](/.attachments/image-6dbb8df8-b8b5-4d00-960d-9e7c358e5fe9.png)

**Output:**

```
{
  "Bins": [
    {
      "BinCode": "STO-1",
      "LocationCode": "WMS"
    },
    {
      "BinCode": "STO-2",
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
