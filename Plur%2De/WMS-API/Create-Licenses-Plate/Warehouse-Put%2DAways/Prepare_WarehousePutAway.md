**ProcessMethod**: Prepare_WarehousePutAway

**Description**:
Prepare_WarehousePutAway

This method is used in the Put Away, in the scenario that the user wishes to update the Bin of an LP before posting the Put-Away.

The purpose of this method is to fragment the lines of a Warehouse Put away into several lines that coincide with the assigned LPs, allowing the possibility of updating each LP Single separately.

Note: This method must be called before editing the Bin of LPs assigned to a Warehouse Put Away.

**Input**:
**Parameters**: 
-	**No**: Warehouse Put Away number.

**Output**:  The output is the information of new lines of a Warehouse Put Away, and although only the Key (Activity Type, Line No, No) is needed to perform any search, it has been decided to further detail the information with the following fields.

-	**ActivityType** : Since the table is really called Warehouse Activity Line, and it works for both Put Aways and Shipments, the type that allows it to be differentiated are included, which are the following:
**'Put-away'**, **'Pick'**, **'Movement'**, **'Invt. Put-away'**,**'Invt. Pick'**, **'Invt. Movement**
-	**No** :Warehouse Put Away number.
-	**ItemNo** : Item No related.
-	**LineNo** : Number  Line.
-	**ZoneCode** : Zone
-	**LocationCode** : Location
-	**BinCode** : Bin
-	**Quantity** : Quantities
-	**LP** : Licensen Plate Number
 
**Warehouse Put Away**
![image.png](/.attachments/image-50a3934e-aff3-4527-9959-7bcb2b47125a.png)

**Post Auto Split (Prepare_WarehousePutAway)**
![image.png](/.attachments/image-fd850ff4-ea23-4a97-a371-78933c9b2053.png)


**Example**:

**Request:**

```
{
  "ProcessMethod": "Prepare_WarehousePutAway",
  "Parameters": [
    {
      "No": "WHSE PUTAWAY-00020"
    }
  ]
}
```

Outputs:

```
{
  "WarehousePutAwayLines": [
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "20000",
      "ZoneCode": "STO",
      "LocationCode": "WMS",
      "BinCode": "FLOOR",
      "Quantity": 2.0,
      "LP": "LP-00140"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "20039",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00139"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "20078",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00138"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "20156",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00137"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "20312",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00136"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "20625",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00135"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "21250",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00134"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "22500",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00133"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "25000",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00132"
    },
    {
      "ActivityType": "Put-Away",
      "No": "WHSE PUTAWAY-00020",
      "ItemNo": "1896-S",
      "LineNo": "30000",
      "ZoneCode": "",
      "LocationCode": "WMS",
      "BinCode": "",
      "Quantity": 2.0,
      "LP": "LP-00131"
    }
  ]
}
```

**Errors**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Put-Away does not exist""
  }
}
```

