**ProcessMethod**: SplitPutAwayLine

**Description**:

Enable that the items can be taken or placed in more than one bin, for example, because the quantity in the suggested bin is insufficient to pick or move or there is not enough room to put away the required quantity.

**Input**:
**Parameters**: 
-	**No**: Warehouse Put Away number.
-	**ItemNo** : Item No related.
-	**LineNo** : Number  Line.
-	**ZoneCode** : Zone
-	**LocationCode** : Location
-	**BinCode** : Bin
-	**QtyToHandle** : Quantities to divide.

 
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
-	**Qty_to_Handle** : Quantities
 
**Warehouse Put Away Line**
![image.png](/.attachments/image-73b97d81-a12a-4952-bb95-563bb80607a6.png)

**Split (Prepare_WarehousePutAway)**
![image.png](/.attachments/image-b2861d37-f2de-42dd-8a48-8432ded0bff9.png)


**Example**:

**Request:**

```
{
  "ProcessMethod": "SplitPutAwayLine",
  "Parameters": [
    {
      "No": "WHSE PUTAWAY-00001",
      "LocationCode": "WMS",
      "LineNo": "40000",
      "ItemNo": "1900-S",
      "BinCode": "STO2",
      "QtyToHandle": "8"
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

