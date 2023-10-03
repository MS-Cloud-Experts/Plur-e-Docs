**ProcessMethod**: CreateBatch_SN_inWR

**Description**: Method that allows to create Serials from the last serial of item


**Parameters:** 
-	**WarhouseReceiptNo**: Warhouse Receipt number.
-	**LineNo**: Line No
-	**QtyToCreate**: Number of serial numbers to be created


**Request:**
```

"jsonRequest":"{"ProcessMethod":"CreateBatch_SN_inWR","Parameters":[{"WarhouseReceiptNo":"WHSE REC-00017","LineNo":"10000","QtyToCreate":"2"}]}"

```

**Output**:

```
{
  "The series was created": true
}
```
