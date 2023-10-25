**Request:** 

```
{
  "ProcessMethod": "UpdateBin_WarehousePickLine",
  "Parameters": [
    {
      "WhseDocumentNo": "WHSE SHIP-00005"
    }
  ]
}
```


**Output** :
```
{
  "WarehousePicks": {
    "WarehousePickHeader": [
      {
        "No": "WHSE PICK-00010",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "",
        "AssignmentDate": "0001-01-01",
        "WarehousePickLines": [
          {
            "actionType": "Take",
            "No": "WHSE PICK-00010",
            "LineNo": 10000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101010",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "ItemNo": "1896-S",
            "Quantity": 10.0,
            "QtyToHandle": 10.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00010",
            "LineNo": 20000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101010",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "ItemNo": "1896-S",
            "Quantity": 10.0,
            "QtyToHandle": 10.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          },
          {
            "actionType": "Take",
            "No": "WHSE PICK-00010",
            "LineNo": 30000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101010",
            "SourceLineNo": 20000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-3",
            "ZoneCode": "STO",
            "ItemNo": "1900-S",
            "Quantity": 10.0,
            "QtyToHandle": 10.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00010",
            "LineNo": 40000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101010",
            "SourceLineNo": 20000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "ItemNo": "1900-S",
            "Quantity": 10.0,
            "QtyToHandle": 10.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          }
        ]
      }
    ]
  }
}
```
