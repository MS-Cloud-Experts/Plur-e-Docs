**ProcessMethods**: 

Para un Warehouse Shipment:
- GetWarehouseShipment

Para la lista de Warehouse Shipments
- GetWarehouseShipments

**Description**:

The **GetWarehouseShipments** method allows to fetch the list of Warehouse Shipments associated to a user.

The **GetWarehouseShipment** method allows to fetch a specific Warehouse shipment with its lines.

**Parameters**: 

GetWarehouseShipment
-	**No**: Warehouse Shipment No.


GetWarehouseShipments
-	**assigned_user_id**: User Id.





**Example**:

Request GetWarehouseShipment:
```
{
  "ProcessMethod": "GetWarehouseShipment",
  "Parameters": [
    {
      "No": "WHSE SHIP-00002"
    }
  ]
}
```
Request GetWarehouseShipments:
```
{
  "ProcessMethod": "GetWarehouseShipments",
  "Parameters": [
    {
      "assigned_user_id": ""
    }
  ]
}
```

**Output GetWarehouseShipment**
```
{
  "WarehouseShipment": {
    "WarehouseShipmentHeader": [
      {
        "No": "WHSE SHIP-00002",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE SHIP",
        "BinCode": "SHIP-1",
        "ZoneCode": "SHIP",
        "PostingDate": "2023-07-18",
        "ShippingAgentCode": "DHL",
        "ShippingAgentServiceCode": "",
        "ShipmentMethodCode": "",
        "ShipmentDate": "2023-07-18",
        "Status": 0,
        "WarehouseShipmentLines": [
          {
            "No": "WHSE SHIP-00002",
            "LineNo": 10000,
            "SourceType": 37,
            "SourceSubtype": 1,
            "SourceNo": "S-ORD101036",
            "SourceLineNo": 10000,
            "LocationCode": "NEWWMS",
            "BinCode": "SHIP-1",
            "ZoneCode": "SHIP",
            "ItemNo": "1988-S",
            "Quantity": 100.0,
            "QtyBase": 100.0,
            "QtyOutstanding": 100.0,
            "QtyOutstandingBase": 100.0,
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
**Output GetWarehouseShipments**
```
{
  "WarehouseShipment": {
    "WarehouseShipmentHeader": [
      {
        "No": "WHSE SHIP-00002",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE SHIP",
        "BinCode": "SHIP-1",
        "ZoneCode": "SHIP",
        "PostingDate": "2023-07-18",
        "ShippingAgentCode": "DHL",
        "ShippingAgentServiceCode": "",
        "ShipmentMethodCode": "",
        "ShipmentDate": "2023-07-18",
        "Status": 0
      },
      {
        "No": "WHSE SHIP-00003",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE SHIP",
        "BinCode": "SHIP-1",
        "ZoneCode": "SHIP",
        "PostingDate": "2023-07-18",
        "ShippingAgentCode": "",
        "ShippingAgentServiceCode": "",
        "ShipmentMethodCode": "",
        "ShipmentDate": "2023-07-18",
        "Status": 1
      },
      {
        "No": "WHSE SHIP-00004",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE SHIP",
        "BinCode": "SHIP-1",
        "ZoneCode": "SHIP",
        "PostingDate": "2023-07-18",
        "ShippingAgentCode": "",
        "ShippingAgentServiceCode": "",
        "ShipmentMethodCode": "",
        "ShipmentDate": "2023-07-18",
        "Status": 1
      },
      {
        "No": "WHSE SHIP-00005",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE SHIP",
        "BinCode": "SHIP-1",
        "ZoneCode": "SHIP",
        "PostingDate": "2023-07-18",
        "ShippingAgentCode": "",
        "ShippingAgentServiceCode": "",
        "ShipmentMethodCode": "",
        "ShipmentDate": "2023-07-18",
        "Status": 1
      },
      {
        "No": "WHSE SHIP-00006",
        "LocationCode": "NEWWMS",
        "NoSeries": "WHSE SHIP",
        "BinCode": "SHIP-1",
        "ZoneCode": "SHIP",
        "PostingDate": "2023-07-18",
        "ShippingAgentCode": "",
        "ShippingAgentServiceCode": "",
        "ShipmentMethodCode": "",
        "ShipmentDate": "2023-07-18",
        "Status": 1
      }
    ]
  }
}

```
