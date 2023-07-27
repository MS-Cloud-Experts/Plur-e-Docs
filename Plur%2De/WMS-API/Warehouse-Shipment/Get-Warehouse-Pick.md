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
        "No": "WHSE PICK-00001",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "",
        "AssignmentDate": "0001-01-01",
        "WarehousePickLines": [
          {
            "No": "WHSE PICK-00001",
            "LineNo": 10000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101038",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "ItemNo": "1006",
            "Quantity": 10.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          },
          {
            "No": "WHSE PICK-00001",
            "LineNo": 20000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101038",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "ItemNo": "1006",
            "Quantity": 10.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          },
          {
            "No": "WHSE PICK-00001",
            "LineNo": 30000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101038",
            "SourceLineNo": 20000,
            "LocationCode": "NEWWMS",
            "BinCode": "STO-4",
            "ZoneCode": "STO",
            "ItemNo": "1007",
            "Quantity": 10.0,
            "QtyToHandle": 0.0,
            "QtyHandled": 0.0,
            "QtyBase": 10.0,
            "QtyOutstanding": 10.0,
            "QtyOutstandingBase": 10.0,
            "UnitofMeasureCode": "PCS",
            "QtyperUnitofMeasure": 1.0,
            "VariantCode": ""
          },
          {
            "No": "WHSE PICK-00001",
            "LineNo": 40000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101038",
            "SourceLineNo": 20000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "ItemNo": "1007",
            "Quantity": 10.0,
            "QtyToHandle": 0.0,
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
