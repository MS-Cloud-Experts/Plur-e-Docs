**ProcessMethod**: Merge

**Description**:
This method allows you to split an existing License Plate into a new one.

**Input**:
Parameters: 
-	**NewLicensePlateCode**: Represents the code of the new License Plate to which the new quantities will be assigned. To create a new License Plate you must use this method:  [GenerateEmptyLP](/Plur%2De/WMS-API/Splits/GenerateEmptyLP)

-	**NewQuantity**: Represents the decimal amounts that will be transferred to the new LP.
-	**OriginalQuantityModified**: It represents the decimal quantities that remained from the original LP, that is, if at the beginning there were 10 units, and in the "NewQuantity" parameter 1 unit was transferred, then this parameter should be sent 9.
-	**OriginalLicensePlateCode**: Represents the License Plate No of the original LP.

**Ouput**: List of License Plates filtered by Item No.



**Example**:

To make a split we must first consult our original LP.

**Request**:

```
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP000535"
    }
  ]
}
```

**Output GetLicencesPlate:**
![image.png](/.attachments/image-10381964-fbc5-48ed-8a94-81a8e68d2064.png)

**License Plate in Business Central:**
![image.png](/.attachments/image-ca56f4ad-94f5-42cc-a8a3-02a626927018.png)


Once the amounts of the LP have been obtained, we could already know the maximum amounts to divide and execute the Split process


**Request:**
```
{
  "ProcessMethod": "Split",
  "Parameters": [
    {
      "NewLicensePlateCode": "LP000777",
      "NewQuantity": "1",
      "OriginalQuantityModified": "2",
      "OriginalLicensePlateCode": "LP000535"
    }
  ]
}
```

**Note**: the amounts in **NewQuantity** and in **OriginalQuantityModified** can never be greater than the original amounts on the LP.

**This would be the equivalent in Buesiness Central:**
![image.png](/.attachments/image-7633550e-9111-45ad-b374-fe695ce7d4fc.png)

In the image we see the field marked in yellow "**New Quantity**" this would be what should be left to our original LP, and it is the parameter **OriginalQuantityModified** that we will pass to our Request.

The output will contain the post number of the 2 internal transactions that are executed. The input on the new LP and the output on the Original LP.

**Outputs:**
```
{
  "Result_AjustOriginal": "{\"Posted\":527}",
  "Result_AjustNew": "{\"Posted\":528}"
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





