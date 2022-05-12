**ProcessMethod**: GetLicencesPlatesByItemNo

**Description**:
Method to return a list of License Plates based on the ItemNo filter.

**Input**:
Parameters: 
-	ItemNo: Represents the number of the Item to which an LP has been assigned.

**Ouput**: List of License Plates filtered by Item No.

-	**LicensePlatesHeaders**: Array of License Plates Headers.

**Example**:

**Request**:


```
{
  "ProcessMethod": "GetLicencesPlate",
  "Parameters": [
    {
      "No": "LP000555"
    }
  ]
}
```


   
```
{
  "ProcessMethod": "Split",
  "Parameters": [
    {
      "NewLicensePlateCode": "LP000776",
      "NewQuantity": "1",
      "OriginalQuantityModified": "1",
      "OriginalLicensePlateCode": "LP000555"
    }
  ]
}
```


Outputs:

![image.png](/.attachments/image-b17f021c-781d-4395-90ba-febe6dd9a647.png)

![image.png](/.attachments/image-9b9ba8d0-1eb3-4caa-8bf3-53e204ef542e.png)


![image.png](/.attachments/image-1308e655-084c-4096-aa82-684e8bea5092.png)