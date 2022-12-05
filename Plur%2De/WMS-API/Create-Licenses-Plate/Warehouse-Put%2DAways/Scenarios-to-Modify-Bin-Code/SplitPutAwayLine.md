**ProcessMethod**: SplitPutAwayLine

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
**'Put-away'**, **'Pick'**, **'Movement'**, **'Invt. Put-away'**,**'Invt. Pick'**, 
**'Invt. Movement**

The values of this field will be treated as Integers, this being the following mapping:

```
**"Put-away"**:= 1;
**"Pick"** :=   2;
**"Movement"** :=   3; 
**"Invt. Put-away"** := 4; 
**"Invt. Pick"**:= 5; 
**"Invt. Movement"**:= 6;
```


-	**No** :Warehouse Put Away number.
-	**ItemNo** : Item No related.
-	**LineNo** : Number  Line.
-	**ZoneCode** : Zone
-	**LocationCode** : Location
-	**BinCode** : Bin
-	**Quantity** : Quantities
-	**LP** : Licensen Plate Number
 
**Warehouse Put Away**
![image.png](/.attachments/image-73b97d81-a12a-4952-bb95-563bb80607a6.png)

**Split (Prepare_WarehousePutAway)**
![image.png](/.attachments/image-b2861d37-f2de-42dd-8a48-8432ded0bff9.png)


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
[
  {
    "ActivityType": 1,
    "No": "WHSE PUTAWAY-00001",
    "ItemNo": "1900-S",
    "LineNo": "40000",
    "ZoneCode": "STO",
    "LocationCode": "WMS",
    "BinCode": "STO-2",
    "Quantity": 8.0,
    "Qty_to_Handle": 8.0
  },
  {
    "ActivityType": 1,
    "No": "WHSE PUTAWAY-00001",
    "ItemNo": "1900-S",
    "LineNo": "45000",
    "ZoneCode": "",
    "LocationCode": "WMS",
    "BinCode": "",
    "Quantity": 1.0,
    "Qty_to_Handle": 1.0
  },
  {
    "ActivityType": 1,
    "No": "WHSE PUTAWAY-00001",
    "ItemNo": "1900-S",
    "LineNo": "50000",
    "ZoneCode": "",
    "LocationCode": "WMS",
    "BinCode": "",
    "Quantity": 1.0,
    "Qty_to_Handle": 1.0
  }
]
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

