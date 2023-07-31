**ProcessMethods**: 

GetWHSPickInShipments

**Description**:

The **GetWHSPickInShipments** method allows to fetch the list of Warehouse Picks associated to a warehouse shipments.

**Parameters**: 

GetWHSPickInShipments
-	**WhseDocumentNo**: Warehouse Shipment No.





**Action Type**
- Value: 1 ---> "Take"
- Value: 2 ---> "Place"

**Example**:

Request GetWHSPickInShipments:
```
{
  "ProcessMethod": "GetWHSPickInShipments",
  "Parameters": [
    {
      "WhseDocumentNo": "WHSE SHIP-00004"
    }
  ]
}
```

**Output GetWHSPickInShipments**
```
{
  "WarehousePicks": {
    "WarehousePickHeader": [
      {
        "No": "WHSE PICK-00001",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE PICK",
        "AssignedUserID": "",
        "AssignmentDate": "0001-01-01",
        "WarehousePickLines": [
          {
            "actionType": "Take",
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
            "actionType": "Place",
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
            "actionType": "Take",
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
            "actionType": "Place",
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
