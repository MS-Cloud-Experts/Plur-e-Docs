**ProcessMethod**: GetItemInfo

**Description**:
Metodo que permite devolver si un Item esta o no manejado por plure

**Input**:
**Parameters**:  
-	**ItemNo**: Item Number.

**Ouput**: 
-	**ItemNo**:Item that was just consulted
-	**Managed_by_PlurE**: boolean variable that says whether or not it is covered by plure


**Example**:

Request:

```
{
  "ProcessMethod": "GetItemInfo",
  "Parameters": [
    {
      "ItemNo": "1900-S"
    }
  ]
}
```


Outputs:

```
{
  "ItemNo": "1900-S",
  "Managed_by_PlurE": true,
  "Auto_Generate_SN": false,
  "Auto_Generate_LOT": false
}
```
![image.png](/.attachments/image-a8a837aa-56e6-4d9d-9f7e-616bed90832a.png)

**Error**:
```
{
  "Error": {
    "Code": "Not found",
    "Message": "The Item No (190A0-S) was not found"
  }
}
```


