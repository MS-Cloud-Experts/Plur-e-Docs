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
{
  "ProcessMethod": "CreatePackageShipmentSingle",
  "Parameters": [
    {
      "No": "WHSE PICK-00006",
      "Weight": 2,
      "Width": 3,
      "Height": 4,
      "Depth": 5,
      "Status": true,
      "ShippingAgentCode": "DHL",
      "ShippingAgentServiceCode": "DHL",
      "ShippingCost": "20000",
      "PackingDate": "2023-07-27T18:00:00",
      "PackageTrackingNo": "000000077787",
      "PackageLinesArray": [
        {
          "WhsDocumentNo": "WHSE PICK-00006",
          "WhsDocumentLineNo": 20000,
          "SourceNo": "S-ORD101015",
          "ItemCode": "1896-S",
          "VariantCode": "",
          "QtyToHandle": 1
        },
        {
          "WhsDocumentNo": "WHSE PICK-00006",
          "WhsDocumentLineNo": 40000,
          "SourceNo": "S-ORD101015",
          "ItemCode": "1900-S",
          "VariantCode": "",
          "QtyToHandle": 4
        }
      ]
    }
  ]
}
```

