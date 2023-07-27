**Description**:
This is the structure of the Json draft that will be used to send from Business Central/Plure Mobil in order to connect to StartShipping and create the Labels.

**Input**: Array
**Parameters**: 
-	**No**: Warehouse Pick Number
-	**LocationCode**: Location Code (All Packages).
-	**PackagesLines**: It is a Json Array, which contains the dimensions of each packet, as well as the delivery address.
          **No**": 1,
          **ItemNo**: "1896-S",
          **Quantity**: 15.0,
          **WarehouseDocumentNo**: "WHSE PICK-00001",
          **SourceNo**: "S-ORD101009",
          **Weight**: Package Weight,
          **Width**: Package Width,
          **Height**":Package Height,
          **Depth**": Package Depth,
          **Status**: Package Status,
          **PackingDate**: Packing Date,
          **SystemCreatedAt**: "2023-07-27T16:34:14.9730000Z",
          **SystemCreatedBy**: "{59AFF9E0-3CD1-483D-B5C7-D5BFC63289FC}" 
           **ShipToAddress**: 
            Json Object Contains the packet address information, 
            **ShipToName**:  Name Customer,
            **ShipToAddress**: Address 1,
            **ShipToAddress2**: Address 1,
            **ShipToCity**: "City",
            **ShipToCountry_RegionCode**: Country,
            **ShipToCounty**: County
           

**Ouput**: 
-	Post-request Output should return at least Tracking No and Agent Services also in Json format.


**Example**:

Request:
```
{
  "Package": [
    {
      "No": "WHSE PICK-00001",
      "LocationCode": "NEWWMS",
      "PackagesLines": [
        {
          "No": 1,
          "ItemNo": SKU,

          "Quantity": Quantity per package,
          "WarehouseDocumentNo": Warehouse Document No.,
          "SourceNo": Sales Order No.,
          "ShipToAddress": {
            "ShipToName": "Adatum Corporation",
            "ShipToAddress": "192 Market Square",
            "ShipToAddress2": "",
            "ShipToCity": "Atlanta",
            "ShipToCountry_RegionCode": "US",
            "ShipToCounty": "GA"
          },
          "Weight": 15.0,
          "Width": 2.0,
          "Height": 2.0,
          "Depth": 3.0,
          "Status": false,
          "PackingDate": "0001-01-01T00:00:00.0000000",
          "SystemCreatedAt": "2023-07-27T16:34:14.9730000Z",
          "SystemCreatedBy": "{59AFF9E0-3CD1-483D-B5C7-D5BFC63289FC}"
        },
        {
          "No": 2,
          "ItemNo": "1896-S",
          "Quantity": 5.0,
          "WarehouseDocumentNo": "WHSE PICK-00001",
          "SourceNo": "S-ORD101009",
          "ShipToAddress": {
            "ShipToName": "Adatum Corporation",
            "ShipToAddress": "192 Market Square",
            "ShipToAddress2": "",
            "ShipToCity": "Atlanta",
            "ShipToCountry_RegionCode": "US",
            "ShipToCounty": "GA"
          },
          "Weight": 1.0,
          "Width": 3.0,
          "Height": 3.0,
          "Depth": 3.0,
          "Status": false,
          "PackingDate": "0001-01-01T00:00:00.0000000",
          "SystemCreatedAt": "2023-07-27T16:34:40.0030000Z",
          "SystemCreatedBy": "{59AFF9E0-3CD1-483D-B5C7-D5BFC63289FC}"
        }
      ]
    }
  ]
}
```


Outputs:
```
{\"Posted\":391}|{\"Posted\":392}

```
**PostMan:**
![image.png](/.attachments/image-12b7180f-f65f-4931-bc15-f389d522ef01.png)