**ProcessMethod**: SplitPallet_ItemV2

# **UNDER CONSTRUCTION**


**Description**:
This method allows you to split an existing License Plate into a new one.

**Considerations:**

1) You cannot split an LP Single that belongs to an LP Pallet.

2) All Split has to do with the Storage process.


**LP Pallet**: we can divide the quantities of an Item belonging to an LP Single into 2 groups. To do this you need to create a blank LP and from there transfer the quantities.
   Internal Note: Could it be transferred to a Pallet?


**Input**:
Parameters: 
-	**NewLicensePlateCode**: Represents the code of the new **License Plate Pallet** to which the new quantities will be assigned. To create a new License Plate you must use this method:  [GenerateEmptyLP](/Plur%2De/Business-Central-API/WMS/Movements/Splits/GenerateEmptyLP)

-	**NewQuantity**: Represents the decimal amounts that will be transferred to the new LP.
-	**OriginalQuantityModified**: It represents the decimal quantities that remained from the original LP, that is, if at the beginning there were 10 units, and in the "NewQuantity" parameter 1 unit was transferred, then this parameter should be sent 9.
-	**OriginalLicensePlateCode**: Represents the License Plate No of the original LP.

**Ouput**: List of License Plates filtered by Item No.



**Example**:

**Step 1:** 
Create an Empty LP Pallet.

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


**Output New LP Pallet:**
![image.png](/.attachments/image-0f816a7e-2722-4749-bce8-c0fef82e04d6.png)

![image.png](/.attachments/image-31fa6598-ebf2-46f3-92cf-c8604487cee5.png)

**Step 2:**
To make a split we must first consult our original LP.

**Request**:

```
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP000316"
    }
  ]
}
```
**Output GetLicencesPlate:**
![image.png](/.attachments/image-4d80cb32-b508-4fef-afcf-3b789eb1515e.png)

**Step 3:**
**Request:**
```
{
  "ProcessMethod": "SplitPallet_LPSingle",
  "Parameters": [
    {
      "OldLPPalletCode": "LP-01096",
      "NewLPPalletCode": " LP-01052 ",
      "ItemChildArray": [
        {
          "ItemCode": "1000",
          "LineNo": "1000",
          "NewQuantity": "1"
        },
        {
          "ItemCode": "1000",
          "LineNo": "2000",
          "NewQuantity": "1"
        }
      ]
    }
  ]
}
```

**Request in Postman:**
![image.png](/.attachments/image-5f5f44a3-8383-42b2-9d5f-31ed0a789f64.png)


Once the amounts of the LP have been obtained, we could already know the maximum amounts to divide and execute the Split process


**New LP:**
![image.png](/.attachments/image-c7914aaf-2ddf-4ee1-b957-9a14014df07d.png)

**Outputs:**
```
{
  "Result_AjustOriginal": "{\"Posted\":90}",
  "Result_AjustNew": "{\"Posted\":91}"
}
```

**Possible Errors:**

```
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The NewLicensePlateCode LP000555 was not found."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The OriginalLicensePlateCode LP000555 was not found."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The new License Plate LP000776 that will receive the Quantities cannot have lines."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The amounts to be divided in the new License Plate= LP000779 cannot be greater than the Original License Plate=LP000555."
  }
}
```





