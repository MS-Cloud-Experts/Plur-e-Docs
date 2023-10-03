**ProcessMethod**: CreateCustomizedBatch_SN_inWR

**Description**: Method to create customized Serials


**Parameters:** 
-	**WarhouseReceiptNo**: Warhouse Receipt number.
-	**LineNo**: Line No
-	**QtyToCreate**: Number of serial numbers to be created
-	**CustomizedSN**: Example of a customized serial "SNAB0001"



**Request:**
```

"jsonRequest":"{"ProcessMethod":"CreateCustomizedBatch_SN_inWR","Parameters":[{"WarhouseReceiptNo":"WHSE REC-00017","LineNo":"10000","QtyToCreate":"2","CustomizedSN":"SNAB0001"}]}"

```


**Output**:

```
{
  "The series was created": true
}
```


