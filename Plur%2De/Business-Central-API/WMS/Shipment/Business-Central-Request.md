**Description**:
This is the structure of the Json draft that will be used to send from Business Central/Plure Mobil in order to connect to StartShipping and create the Labels.

**Input**: Array
**Parameters**: 
-	**No**: Warehouse Pick Number
-	**LocationCode**: Location Code (All Packages).
-	**PackagesLines**: It is a Json Array, which contains the dimensions of each packet, as well as the delivery address.
          **No**": 1,
          **ItemNo**": SKU,
          **Quantity**": Quantity per Package,
          **WarehouseDocumentNo**: Warehouse Document No.
          **SourceNo**: Sales Order No..
          **Weight**: Package Weight.
          **Width**: Package Width.
          **Height**":Package Height.
          **Depth**": Package Depth.
          **Status**: Package Status.
          **PackingDate**: Packing Date.
          **SystemCreatedAt**: "2023-07-27T16:34:14.9730000Z"
          **SystemCreatedBy**: "{59AFF9E0-3CD1-483D-B5C7-D5BFC63289FC}" 
-	**ShipToAddress**: 
            Json Object Contains the packet address information, 
            **ShipToName**:  Name Customer,
            **ShipToAddress**: Address 1,
            **ShipToAddress2**: Address 2,
            **ShipToCity**: "City",
            **ShipToCountry_RegionCode**: Country,
            **ShipToCounty**: County
           

**Ouput**: 
-	Post-request Output should return at least Tracking No and Agent Services also in Json format.


**Example**:

Request:
```
[
  {
    "PackageHeaders": {
      "No": 1,
      "WarehouseDocumentNo": "WHSE PICK-00005",
      "SourceNo": "S-ORD101011",
      "Weight": 0.0,
      "Width": 0.0,
      "Height": 0.0,
      "Depth": 0.0,
      "Status": false,
      "PackingDate": "0001-01-01T00:00:00.0000000",
      "Lines": [
        {
          "PackageNo": 1,
          "LineNo": 1000,
          "SourceNo": "S-ORD101011",
          "WarehouseDocumentNo": "WHSE PICK-00005",
          "WarehouseLineNo": 20000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1.0
        },
        {
          "PackageNo": 1,
          "LineNo": 2000,
          "SourceNo": "S-ORD101011",
          "WarehouseDocumentNo": "WHSE PICK-00005",
          "WarehouseLineNo": 20000,
          "ItemNo": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1.0
        }
      ],
      "ShipToAddress": {
        "ShipToName": "Adatum Corporation",
        "ShipToAddress": "192 Market Square",
        "ShipToAddress2": "",
        "ShipToCity": "Atlanta",
        "ShipToCountry_RegionCode": "US",
        "ShipToCounty": "GA"
      },
      "SystemCreatedAt": "2023-07-28T15:55:58.9600000Z",
      "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
    }
  }
]
```

