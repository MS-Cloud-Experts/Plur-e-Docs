**ProcessMethod**: Post_WarehousePutAways

**Description**:
Allows you to post a **Warehouse Activity** of type **Put-Away** and convert it into a "**Registered Whse. Activity Hdr.**" **Put-Away** type.

**Parameters**: 

**Input:**
-	**No**: Represents the "Warehouse Activity Header number that you want to post.

**Ouput**: 
This process allows you to register a Warehouse Put-Away (Warehouse Activity of the Put-Away type) in a Registered Warehouse of the Put-Away type.


**Example**:

![image.png](/.attachments/image-8916efd1-5b8d-4898-b34d-964b4a7ea95f.png)

**Request:**

`"jsonRequest":"{"ProcessMethod":"Post_WarehousePutAways","Parameters":[{"No":"107323"}]}"`

**Outputs**:
This method would be the equivalent of "Register Put-Away" the Receipt directly in Business Central.


**Result**:

It will return a number of Registered_Whse_Activity if the post was successful, otherwise an error message.

`{"Registered_Whse_Activity":"10113"}`

**Errors**:

```
{
  "Error": {
    "Code": "Not found",
    "Message": The Warehouse Receipt does not exist"
  }
}
```


