**ProcessMethod**: Post_WarehouseReceipts

**Description**:
Method that allows you to post a Warehouse Receipt and convert it into a Warehouse Put-Away.

**Parameters**: 
No: Allows you to bring a single Warehouse Receipt. 

**Ouput**: Warehouse Put-Away (_Warehouse_Activity_) number generated or Error in case of not being able to post in JSON format.

**Example**:
`"jsonRequest":"{"ProcessMethod":"Post_WarehouseReceipts","Parameters":[{"No":"107323"}]}"`

**Outputs**:

**Posted OK**:

`{"Warehouse_Activity_No":"10113"}`

**Errors**:


```
{"Error":"The Warehouse Receipt does not exist"}
{"Error":"The source document Purchase Order 106040 is not released."}
{"Error":"The Location does not exist. Identification fields and values: Code=''"}
```

