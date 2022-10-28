**ProcessMethod**: SplitLPPallet

UNDER CONSTRUCTION

**Description**:
This method allows you to split an existing License Plate into a new one.

**Considerations:**

1) You cannot split an LP Single that belongs to an LP Pallet.

2) All Split has to do in the Storage process.

**Split Types:**

1) **LP Single**: we can divide the quantities of an Item belonging to an LP Single into 2 groups. To do this you need to create a blank LP and from there transfer the quantities.
   Internal Note: Could it be transferred to a Pallet?

2) **LP Pallet**: in this type we have 3 options:
  2.1) If the LP Pallet has items between its lines, the scenario would be identical to the aforementioned LP Single.
  2.2) If one of the lines is an LP Single, we could create a new LP Pallet, where we would transfer the LP Singles of the Original. Perhaps it should be considered that the original LP Pallet should not be left without lines

**Input**:
Parameters: 
-	**NewLicensePlateCode**: Represents the code of the new License Plate to which the new quantities will be assigned. To create a new License Plate you must use this method:  [GenerateEmptyLP](/Plur%2De/WMS-API/Movements/Splits/GenerateEmptyLP)

-	**NewQuantity**: Represents the decimal amounts that will be transferred to the new LP.
-	**OriginalQuantityModified**: It represents the decimal quantities that remained from the original LP, that is, if at the beginning there were 10 units, and in the "NewQuantity" parameter 1 unit was transferred, then this parameter should be sent 9.
-	**OriginalLicensePlateCode**: Represents the License Plate No of the original LP.

**Ouput**: List of License Plates filtered by Item No.



# **Example**:

To make a split we must first consult our original LP.

**Step 1: GetLicencesPlate** 

![image.png](/.attachments/image-d6f1dd00-47e5-4686-8cfa-267982db5422.png)

**Request**:

```
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP000275"
    }
  ]
}
```

**Step 2: GenerateEmptyLP** 

```
{
  "ProcessMethod": "GenerateEmptyLP",
  "Parameters": [
    {
      "LPType": "Pallet",
      "ZoneCode": "STO",
      "LocationCode": "CCC",
      "BinCode": ""
    }
  ]
}
```

![image.png](/.attachments/image-b93d1077-3f6d-4202-b11a-fa54bfa33129.png)

**Step 3: SplitLPPallet** :

Assuming we want to move the LP Single: **LP-00272**

**Request:**
```
{
  "ProcessMethod": "SplitLPPallet",
  "Parameters": [
    {
      "OldLPPalletCode": "LP-00275",
      "NewLPPalletCode": "LP-00285",
      "LPChildSingleCode": "LP-00272"
    }
  ]
}
```

Possible Errores:

    
```
"error": {
        "code": "Application_DialogException",
        "message": "ProcessMethod SplitLPPallet not found!!  CorrelationId:  e01856f0-8e5b-4af7-b74d-caab5151904f."
    }
```





