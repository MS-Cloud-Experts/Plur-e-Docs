**ProcessMethod**: GetDefaultBin

**Description**:
This method returns the Default Bin used to edit a Put-Away

**Parameters**: 

**Ouput**: Returns list of Bins available to be adjusted in the License Plate
-	**Bins**: is a Json array that contains the Bin Code and Location code to which each possible assignable BIN belongs.

**Example**:

```
**Request:**
{
  "ProcessMethod": "GetDefaultBin",
  "Parameters": []
}
```

![image.png](/.attachments/image-fd904dae-a032-4457-aae2-bec93f3149b9.png)

**Output:**
```
{"Default Location":"WMS","Default Bin":"FLOOR"}
```
