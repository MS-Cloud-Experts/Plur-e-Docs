**Request:** 

```
{
  "ProcessMethod": "CreateWarehousePick",
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
        "No": "WHSE PICK-00093",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "",
        "AssignmentDate": "0001-01-01",
        "WarehousePickLines": [
          {
            "actionType": "Take",
            "No": "WHSE PICK-00093",
            "WhseDocumentNo": "WHSE SHIP-00086",
            "LineNo": 10000,
            "ItemNo": "1906-S",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "ATHENS Mobile Pedestal",
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101121",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-2",
            "BinCodeList": [
              {
                "BinCode": "NOCOUNT"
              },
              {
                "BinCode": "STO-1"
              },
              {
                "BinCode": "STO-2"
              }
            ],
            "ZoneCode": "STO",
            "Quantity": 9.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 9.0,
            "QtyOutstanding": 9.0,
            "QtyOutstandingBase": 9.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00093",
            "WhseDocumentNo": "WHSE SHIP-00086",
            "LineNo": 20000,
            "ItemNo": "1906-S",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "ATHENS Mobile Pedestal",
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101121",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "BinCodeList": [
              {
                "BinCode": "NOCOUNT"
              },
              {
                "BinCode": "STO-1"
              },
              {
                "BinCode": "STO-2"
              }
            ],
            "ZoneCode": "SHIP",
            "Quantity": 9.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 9.0,
            "QtyOutstanding": 9.0,
            "QtyOutstandingBase": 9.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Take",
            "No": "WHSE PICK-00093",
            "WhseDocumentNo": "WHSE SHIP-00086",
            "LineNo": 30000,
            "ItemNo": "1906-S",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "ATHENS Mobile Pedestal",
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101121",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-1",
            "BinCodeList": [
              {
                "BinCode": "NOCOUNT"
              },
              {
                "BinCode": "STO-1"
              },
              {
                "BinCode": "STO-2"
              }
            ],
            "ZoneCode": "STO",
            "Quantity": 70.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 70.0,
            "QtyOutstanding": 70.0,
            "QtyOutstandingBase": 70.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00093",
            "WhseDocumentNo": "WHSE SHIP-00086",
            "LineNo": 40000,
            "ItemNo": "1906-S",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "ATHENS Mobile Pedestal",
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101121",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "BinCodeList": [
              {
                "BinCode": "NOCOUNT"
              },
              {
                "BinCode": "STO-1"
              },
              {
                "BinCode": "STO-2"
              }
            ],
            "ZoneCode": "SHIP",
            "Quantity": 70.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 70.0,
            "QtyOutstanding": 70.0,
            "QtyOutstandingBase": 70.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          }
        ]
      }
    ],
    "WarehousePicksNoCreated": [
      {
        "Item No.": "1906-S",
        "Quantity": 31.0
      }
    ]
  },
  "Duration": "8 seconds 904 milliseconds"
}
```
