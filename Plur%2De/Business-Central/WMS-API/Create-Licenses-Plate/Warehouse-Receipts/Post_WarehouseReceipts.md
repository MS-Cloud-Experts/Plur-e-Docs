**ProcessMethod**: Post_WarehouseReceipts

**Description**:
Allows you to post a Warehouse Receipt and convert it into a Warehouse Activity of the Warehouse Put-Away type.

**Parameters**: 

**Input:**
-	**No**: Represents the Warehouse Receipt number that you want to post.

**Ouput**: 

Warehouse Put-Away (_Warehouse_Activity_) number generated or Error in case of not being able to post in JSON format.

**Example**:

**Request:**

`"jsonRequest":"{"ProcessMethod":"Post_WarehouseReceipts","Parameters":[{"No":"107323"}]}"`

**Outputs**:
This method would be the equivalent of Posting the Receipt directly in Business Central.

![image.png](/.attachments/image-07faa94f-dfd8-41ef-aefb-8989012865b0.png)

**Result**:

It will return a number of Warehouse_Activity_No if the post was successful, otherwise an error message.

`{"Warehouse_Activity_No":"10113"}`

**Errors**:
```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Receipt does not exist."
  }
}
```

