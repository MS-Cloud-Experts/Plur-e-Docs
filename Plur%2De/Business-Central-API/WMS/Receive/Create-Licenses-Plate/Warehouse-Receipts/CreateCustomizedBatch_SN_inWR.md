**ProcessMethod**: CreateCustomizedBatch_SN_inWR

**Description**: It allows to bring a particular Warehouse Receipt through the key field No.


**Parameters:** 
-	**WarhouseReceiptNo**: Warhouse Receipt number.
-	**LineNo**: Line No
-	**No**: Allows you to bring a single Warehouse Receipt.
-	**No**: Allows you to bring a single Warehouse Receipt.



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


