**ProcessMethod**: MoveBinToBinArray_LP

**Description**:
This method allows you to move an Item with its associated LP into the inventory.

**Input**: Array
**Parameters**: 
-	**LPNo**: Number of LP you want to move.
-	**Zone**: Zoneof LP you want to move.
-	**FromBin**: Bin where the LP you want to move is currently located.
-	**ToBin**: Destination bin where you want to move the LP to..
-	**LocationCode**: LP Location.
-	**ItemNo**: Item you want to move.
-	**Qty**: QTY you want to move.
-	**UnitofMeasureCode**: Unit of Measure Code of the License Plate that you want to move.

**Ouput**: 
-	**Posted**: If the output presents the Posted value, it implies that the inventory movement was generated correctly.


**Example**:

Request:
```
[
{
  "ArrayToMove": [
    {
    "LPNo":"LP-00511",
    "Zone":"STO",
    "FromBin":"NOCOUNT",
    "ToBin":"STO-4",
    "LocationCode":"PLURE"
    },
    {
    "LPNo":"LP-00510",
    "Zone":"STO",
    "FromBin":"NOCOUNT",
    "ToBin":"STO-4",
    "LocationCode":"PLURE"
    }
  ]
}
]
```


Outputs:
```
{\"Posted\":391}|{\"Posted\":392}

```
**PostMan:**
![image.png](/.attachments/image-12b7180f-f65f-4931-bc15-f389d522ef01.png)