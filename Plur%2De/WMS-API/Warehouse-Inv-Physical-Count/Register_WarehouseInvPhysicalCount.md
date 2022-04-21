**ProcessMethod**: Register_WarehouseInvPhysicalCount

**Description**:
This method allows you to update the physical quantities counted in a Warehouse Inv Journal.

**Input**:
**Parameters**: 
-	**JournalTemplateName**: JournalTemplateName.
-	**LocationCode**: Specific Location where you want to perform the inventory count.

**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"Register_WarehouseInvPhysicalCount\",\"Parameters\":[{\"JournalTemplateName\":\"PHYSICAL I\",\"LocationCode\":\"CCC\"}]}"`

**Output**: 

```
{
  "Posted": 322
}
```



**Errors:**

`
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The WhseJnlLine was not found in JournalTemplateName=PHYSICAL I and JournalBatchName=PLUR-E."
  }
}
`



