**ProcessMethod**: Merge

**Description**:
This method allows you to split an existing License Plate into a new one.

**Input**:
Parameters: 
-	**LicensePlatesHeadersAddedCode**: It represents the License Plate number that will be used as an aggregator to a base License Plate, that is, this License Plate will transfer its elements to another License Plate (Base) and after the process it must be canceled and without quantities.

-	**LicensePlatesHeadersBaseCode**: Represents the License Plate number that will be used as a base or root in the merge, that is, in this the quantities or elements of another License Plate will be added.


**Ouput**: List of License Plates filtered by Item No.



**Example**:

To make a split we must first consult our original LP.

**Request**:

```
{
  "ProcessMethod": "Merge",
  "Parameters": [
    {
      "LicensePlatesHeadersAddedCode": "LP000820",
      "LicensePlatesHeadersBaseCode": "LP000819"
    }
  ]
}
```

**Outputs:**

```
{
  "Result_AjustOriginal": "{\"Posted\":527}",
  "Result_AjustNew": "{\"Posted\":528}"
}
```

**Output in Business Central:**

![image.png](/.attachments/image-22d13190-1dea-4f12-b276-300a344fc380.png)



**Possible Errors:**

```
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The LicensePlatesHeadersAddedCode LP000555 was not found."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The LicensePlatesHeadersBaseCode LP000555 was not found."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "License Plate LP000555 must be in Storage state to perform the Merge."
  }
}

{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The amounts to be divided in the new License Plate= LP000779 cannot be greater than the Original License Plate=LP000555."
  }
}
```





