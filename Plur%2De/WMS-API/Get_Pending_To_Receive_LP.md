**ProcessMethod**: Get_Pending_To_Receive_LP

**Description**:
This method allows you to obtain the pending License Plates by believing the original Purch Order.

**Input**:
**Parameters**: 
-	**No**: Allows you to bring a single Warehouse Receipt. 
-	**ItemNo**: Warehouse Receipt Number
-	**BinCode**: Bin Code assigned to the product in the Warehouse Receipt.
-	**UnitofMeasureCode**: Unit of measure assigned to the product in the Warehouse Receipt.

**Ouput**: Method that returns the number of assigned and pending LP to be assigned to a Warehouse Receipt.

-	**Created**: Boolean value that indicates if the process that was executed created or assigned a new License Plate. In the case of consulting the number of LP (Licensed Plate) it will always return a false value.
-	**Message**: Used to return messages returned by Business Central, possibly when an error is generated.
-	**LP_Pending_To_Receive**: Number of pending LP still to be assigned in the Purch Order / Warehouse Receipt.
-	**LP_Received**: Number of assigned LP assigned in the Warehouse Receipt.

**Example**:

**LP_Pending_To_Receive**:
![image.png](/.attachments/image-84ebc2c6-b814-4ac6-b25b-e2c6969c18a0.png)

The difference between the number of labels created minus the total amounts to Receive gives the number of Pending to Receive, necessary to be able to show the user how many can still be created.
![image.png](/.attachments/image-4a311178-fc10-4dd2-bd3f-7cf766fd4785.png)

**Request:**
`"jsonRequest":"{"ProcessMethod":"Get_Pending_To_Receive_LP","Parameters":[{"No":"107327","ItemNo":"ItemPLU1","BinCode":"","UnitofMeasureCode":"PCS"}]}"`

**Outputs**:

`"{"Created":false,"Message":"","LP_Pending_To_Receive":5.0,"LP_Received":""}"`

**Errors**:

`{"Error":"The Warehouse Receipt does not exist"}`
