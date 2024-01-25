**ProcessMethod**: GetWarehouseReceipts

**Description**:
Allows you to bring a list of open Warehouse Receipts to be posted in a Warehouse Activity (Warehouse Put-Away) or assign a License Plate.

**Parameters**: 

**Input**:

**Parameters**: 
-	**assigned_user_id**: filter that allows obtaining only the warehouse receipts of a user. If it is left blank, it brings all the existing ones.

**Ouput**: Returns an array of Warehouse Receipts in Json format.

-	**WarehouseReceipts**: Returns an array of Warehouse Receipts expressed in the key: `WarehouseReceipts`

**Example**:

**Request:**
`"jsonRequest":"{"ProcessMethod":"GetWarehouseReceipts","Parameters":[{"assigned_user_id":""}]}"`

**Error**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Receipt List is Empty."
  }
}
```
**Output**:

**WarehouseReceipts:**

![image.png](/.attachments/image-eaca9fc1-e4fe-46d1-86ad-2b28cb94e452.png)

**Output:**

```
{
  "WarehouseReceipts": [
    {
      "AssignmentDate": "2024-01-11",
      "No": "WHSE REC-00006",
      "LocationCode": "MAIN"
    }
  ],
  "WarehouseReceiptLines": [
    [
      {
        "No": "WHSE REC-00006",
        "LineNo": 10000,
        "SourceType": 39,
        "SourceSubtype": 1,
        "SourceDocument": "Purchase Order",
        "SourceNo": "PO-109906",
        "SourceLineNo": 10000,
        "LocationCode": "MAIN",
        "BinCode": "MAIN",
        "ZoneCode": "REC",
        "ItemNo": "K4KOAETHE",
        "Quantity": 100.0,
        "QtyBase": 100.0,
        "QtyOutstanding": 100.0,
        "QtyOutstandingBase": 100.0,
        "QtytoReceive": 0.0,
        "QtytoReceiveBase": 0.0,
        "QtyReceived": 0.0,
        "QtyReceivedBase": 0.0,
        "UnitofMeasureCode": "EA",
        "QtyperUnitofMeasure": 1.0,
        "VariantCode": "005003",
        "OverReceiptQuantity": 0.0,
        "OverReceiptCode": "",
        "Managed_by_PlurE": false,
        "Auto_Generate_SN": false,
        "Auto_Generate_LOT": false,
        "ItemTrackingCode": "SERIAL",
        "LPArray": {
          "LicensePlates": []
        },
        "PLUNoLPCreated": 0.0,
        "PLULPSingles": "",
        "PLULPPalletChildsasLP": "",
        "PLUNewQtyOutstanding": 0.0
      }
    ]
  ]
}
```

