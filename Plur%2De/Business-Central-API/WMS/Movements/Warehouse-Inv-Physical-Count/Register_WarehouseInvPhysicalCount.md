**ProcessMethod**: PreRegister_WarehouseInvPhysicalCount

**Description**:
This method allows registering a Batch of physical inventory count, generating in turn the update of the Warehouse Entry and the associated License Plates.

**Input**:
-	**JournalTemplateName**: Specific JournalTemplateNamewhere you want to perform the inventory count.
-	**JournalBatchName**: Specific JournalBatchName where you want to perform the inventory count.
-	**LocationCode**: Specific Location where you want to perform the inventory count.
 
**Example**:

Request:

 
```
{
  "ProcessMethod": "Register_WarehouseInvPhysicalCount",
  "Parameters": [
    {
      "JournalTemplateName": "PHYSICAL I",
      "JournalBatchName": "DARIO",
      "LocationCode": "WMS"
    }
  ]
}
```


**Warehouse Physical Inventory Journal to Register**:
![image.png](/.attachments/image-dd9ad69c-3a71-4685-8f1e-fe29d2bf518d.png)

**Output**: 
-	**Posted**: Return a value if the process was registered successfully.

```
  "value": "{\"Posted\":325}"
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


