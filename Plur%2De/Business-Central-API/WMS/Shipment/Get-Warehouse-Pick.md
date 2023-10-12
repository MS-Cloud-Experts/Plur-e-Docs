**ProcessMethods**: 

For a Warehouse Pick:
- GetWarehousePick

For the Warehouse Picks list
- GetWarehousePicks

**Description**:

The **GetWarehousePicks** method allows to fetch the list of Warehouse Picks associated to a user.

The **GetWarehousePick** method allows to fetch a specific Warehouse Picks with its lines.

**Parameters**: 

GetWarehousePick
-	**No**: Warehouse Pick No.


GetWarehousePicks
-	**assigned_user_id**: User Id.



**Action Type**
- Value: 1 ---> "Take"
- Value: 2 ---> "Place"

**Example**:

Request GetWarehousePick:
```
{
  "ProcessMethod": "GetWarehousePick",
  "Parameters": [
    {
      "No": "WHSE PICK-00001"
    }
  ]
}
```
Request GetWarehousePicks:
```
{
  "ProcessMethod": "GetWarehousePicks",
  "Parameters": [
    {
      "assigned_user_id": "DARIO.SANCHEZ"
    }
  ]
}
```

**Output GetWarehousePick**
```
{
  "WarehousePick": {
    "WarehousePickHeader": [
      {
        "No": "WHSE PICK-00042",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "DARIO.SANCHEZ",
        "AssignmentDate": "2023-10-11",
        "WarehousePickLines": [
          {
            "actionType": "Take",
            "No": "WHSE PICK-00042",
            "LineNo": 10000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "SN99",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00042",
            "LineNo": 20000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "SN99",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Take",
            "No": "WHSE PICK-00042",
            "LineNo": 30000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "SN1",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00042",
            "LineNo": 40000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "SN1",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Take",
            "No": "WHSE PICK-00042",
            "LineNo": 50000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "SN2",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00042",
            "LineNo": 60000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "SN2",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Take",
            "No": "WHSE PICK-00042",
            "LineNo": 70000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00042",
            "LineNo": 80000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Take",
            "No": "WHSE PICK-00042",
            "LineNo": 90000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          },
          {
            "actionType": "Place",
            "No": "WHSE PICK-00042",
            "LineNo": 100000,
            "ItemNo": "1006",
            "VariantCode": "",
            "SerialNo": "",
            "LotNo": "",
            "Description": "1006",
            "SourceType": 5741,
            "SourceSubtype": 0,
            "SourceNo": "1007",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "Quantity": 1.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 1.0,
            "QtyOutstanding": 1.0,
            "QtyOutstandingBase": 1.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0
          }
        ]
      }
    ],
    "SerialAvailable": [
      {
        "LotNo": "",
        "SerialNo": "SN1",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN10",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN1000",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN1001",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN1002",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN1003",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN1004",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN11",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN12",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN13",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN14",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN15",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN18",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN19",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN198",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN199",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN2",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN20",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN2000",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN2001",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN2002",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN2003",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN2005",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN21",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN22",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN3",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN30",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN31",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN32",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN33",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN34",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN4",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN5",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN50",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN51",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN52",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN53",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN54",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN55",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN56",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN57",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN58",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN59",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN6",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN60",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN61",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN62",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN63",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN64",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN65",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN66",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN67",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN68",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN69",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN7",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN70",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN71",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN72",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN73",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN74",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN75",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN76",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN77",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN78",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN79",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN8",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN80",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN81",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN82",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN83",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN84",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN85",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN86",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN87",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN88",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN89",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN9",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN90",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN91",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN92",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN93",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN94",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN95",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN96",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN97",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN98",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      },
      {
        "LotNo": "",
        "SerialNo": "SN99",
        "TotalQuantity": "1",
        "CurrentPendingQuantity": "0",
        "TotalAvailableQuantity": "1"
      }
    ],
    "LotAvailable": []
  }
}

```
**Output \"GetWarehousePicks**
```
{
  "WarehousePicks": {
    "WarehousePickHeader": [
      {
        "No": "WHSE PICK-00002",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "DARIO.SANCHEZ",
        "AssignmentDate": "2023-07-26"
      }
    ]
  }
}

```
or

```
{
  "WarehousePicks": {
    "WarehousePickHeader": [
      {
        "No": "WHSE PICK-00001",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "",
        "AssignmentDate": "0001-01-01"
      },
      {
        "No": "WHSE PICK-00003",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "",
        "AssignmentDate": "0001-01-01"
      }
    ]
  }
}

```
