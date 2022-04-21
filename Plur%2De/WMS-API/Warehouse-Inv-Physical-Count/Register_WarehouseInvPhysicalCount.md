**ProcessMethod**: Register_WarehouseInvPhysicalCount

**Description**:
This method allows you to update the physical quantities counted in a Warehouse Inv Journal.

**Input**:
**Parameters**: 
-	**JournalTemplateName**: JournalTemplateName.
-	**LocationCode**: Specific Location where you want to perform the inventory count.

**Example**:

Request:

`"jsonRequest":"{\"ProcessMethod\":\"Register_WarehouseInvPhysicalCount\",\"Parameters\":[{\"JournalTemplateName\":\"PHYSICAL I\",\"LocationCode\":\"BBB\"}]}"`

**Output**: 

```
{
  "Posted": 322
}
```

**Licenses Plate Ledger Entries:**
![image.png](/.attachments/image-59b91d75-849a-4de7-9268-1e2224720718.png)

**Bin Contents:**

![image.png](/.attachments/image-3b2fdb8d-771c-49ff-975e-aac713eb80f5.png)


**Errors:**

`
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The WhseJnlLine was not found in JournalTemplateName=PHYSICAL I and JournalBatchName=PLUR-E."
  }
}
`



