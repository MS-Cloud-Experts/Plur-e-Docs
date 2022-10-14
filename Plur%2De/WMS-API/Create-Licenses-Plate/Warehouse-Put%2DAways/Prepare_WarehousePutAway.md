**ProcessMethod**: Prepare_WarehousePutAway

**Description**:
This method returns the elements of the table "Warehouse Activity Header" filtered so that only "Put-Away" is visible. In this case, the filtered record is brought in the "No" field. returning the "Warehouse Activity Header" and the "Warehouse Activity Line" in JSON format.

Note: There is a table called " Warehouse Activity Header" which contains all registered Put-Aways and Pick, changing only the Type for differences between one or the other.

**Input**:
**Parameters**: 
-	**No**: Allows you to bring a single Warehouse Activity Header. 

**Ouput**:  

-	**WarehousePutAways**: Contains a Registered `WarehousePutAwayHeader` and an array of lines expressed in the key: `WarehouseActivityLine`.
-	
 
**Warehouse Put Away**
![image.png](/.attachments/image-50a3934e-aff3-4527-9959-7bcb2b47125a.png)

**Post Auto Split (Prepare_WarehousePutAway)**
![image.png](/.attachments/image-cf694d91-f263-4aee-90ab-805814040a8b.png)


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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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
      "ActivityType": "Place",
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

