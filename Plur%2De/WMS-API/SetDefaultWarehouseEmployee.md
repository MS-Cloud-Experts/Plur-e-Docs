**ProcessMethod**: SetDefaultWarehouseEmployee

**Description**:
This method allows you to configure the default location of a warehouse employee.


**Input**:
**Parameters**: 
-	**UserID**: represents the ID of the user whose Default is to be updated.
-	**LocationCode**: represents the location of the user whose Default is to be updated.
-	**Default**: Boolean value that will update the Default of the warehouse employee.

Note: before activating a default for a new location, it cannot be active for a previous one, otherwise it will give an error when executing the method.

**Ouput**: 
-	**Result**: Returns all the fields related to the record that was just updated.

**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"SetDefaultWarehouseEmployee\",\"Parameters\":[{\"UserID\":\"IVAN.LABRADOR1\",\"LocationCode\":\"MAIN WMS\",\"Default\":\"true\"}]}"`

Outputs:


```
{
  "Result": [
    {
      "id": 7301,
      "name": "WarehouseEmployee",
      "company": "CRONUS USA, Inc.",
      "position": "User ID=CONST(IVAN.LABRADOR1),Location Code=CONST(MAIN WMS)",
      "recordId": "Warehouse Employee: IVAN.LABRADOR1,MAIN WMS",
      "primaryKey": {
        "fieldCount": 2,
        "fields": [
          {
            "id": 1,
            "name": "UserID",
            "type": "Code",
            "value": "IVAN.LABRADOR1",
            "System": false
          },
          {
            "id": 2,
            "name": "LocationCode",
            "type": "Code",
            "value": "MAIN WMS",
            "System": false
          }
        ]
      },
      "fieldCount": 9,
      "fields": [
        {
          "id": 1,
          "name": "UserID",
          "type": "Code",
          "value": "IVAN.LABRADOR1",
          "System": false
        },
        {
          "id": 2,
          "name": "LocationCode",
          "type": "Code",
          "value": "MAIN WMS",
          "System": false
        },
        {
          "id": 4,
          "name": "Default",
          "type": "Boolean",
          "value": true,
          "System": false
        },
        {
          "id": 7710,
          "name": "ADCSUser",
          "type": "Code",
          "value": null,
          "System": false
        },
        {
          "id": 2000000000,
          "name": "$systemId",
          "type": "GUID",
          "value": "{42B73F37-2E94-EC11-80F2-000D3A74F212}",
          "System": false
        },
        {
          "id": 2000000001,
          "name": "SystemCreatedAt",
          "type": "DateTime",
          "value": "2022-02-22T22:24:36.797Z",
          "System": false
        },
        {
          "id": 2000000002,
          "name": "SystemCreatedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": false
        },
        {
          "id": 2000000003,
          "name": "SystemModifiedAt",
          "type": "DateTime",
          "value": "2022-03-22T22:32:51.367Z",
          "System": false
        },
        {
          "id": 2000000004,
          "name": "SystemModifiedBy",
          "type": "GUID",
          "value": "{C8466A18-3206-4894-8B37-3ABD69030D7D}",
          "System": false
        }
      ]
    }
  ]
}

{
  "Error": {
    "Code": "Not found",
    "Message": "The Item No (190a0-S) was not found"
  }
}
```
'Error', 'Warehouse Employee does not exist.

