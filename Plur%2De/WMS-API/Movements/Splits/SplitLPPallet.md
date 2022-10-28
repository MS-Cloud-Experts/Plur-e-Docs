**ProcessMethod**: SplitLPPallet

**Description**:
This method allows you to split an existing License Plate into a new one.

**Considerations:**

1) You cannot split an LP Single that belongs to an LP Pallet.

2) All Split has to do in the Storage process.

**Split Types:**

 **LP Pallet**: in this type we have 3 options:
  1) If the LP Pallet has items between its lines, the scenario would be identical to the aforementioned LP Single ----> [This Link.](https://dev.azure.com/MSCloudExperts/Plur-e/_wiki/wikis/Plur-e.wiki/66/SplitLPSingle)

  2) If one of the lines is an LP Single, we could create a new LP Pallet, where we would transfer the LP Singles of the Original. Perhaps it should be considered that the original LP Pallet should not be left without lines

**Input**:
Parameters: 
-	**OldLPPalletCode**: Represents the LP Pallet of Origin, from which the user is going to get an LP Single.
-	**NewLPPalletCode**: Represents the Destination LP Pallet, which the user is going to insert the LP Single.
-	**LPChildSingleCode**:  It is the LP Single child of the LP Pallet Original that is going to be moved.



To create a new License Plate you must use this method:  [GenerateEmptyLP](/Plur%2De/WMS-API/Movements/Splits/GenerateEmptyLP)


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

**Ouput:**

```
{
  "Result": true,
  "Message": "Ok"
}
```

**Old Pallet:**
![image.png](/.attachments/image-330e28ed-04ae-401d-8397-3a677ddd46b2.png)

**New Pallet:**
![image.png](/.attachments/image-4e07238c-31d7-4d30-a5d5-e7ac87d5198a.png)


**Possible Errors:**


```
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The OldLPPalletCode LP-002751 was not found."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The NewLPPalletCode LP-00275 was not found."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The LPChildSingleCode LP-00275 was not found."
  }
}
```

    






