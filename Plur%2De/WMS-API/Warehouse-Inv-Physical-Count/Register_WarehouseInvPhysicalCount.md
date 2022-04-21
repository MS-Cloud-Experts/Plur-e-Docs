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
-The process will be executed correctly if it returns Yes.



