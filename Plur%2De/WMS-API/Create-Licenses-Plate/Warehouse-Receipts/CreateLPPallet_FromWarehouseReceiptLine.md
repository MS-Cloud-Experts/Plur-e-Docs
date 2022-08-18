**ProcessMethod**: CreateLPPallet_FromWarehouseReceiptLine

**Description**:
This method allows you to generate License Plates within Business Central associated with a Warehouse Receipt.

The output of this method returns the LP Document No Pallet Generated.

**Input**:

**Parameters**: 
-	**No**: Represents the Warehouse Receipt number to which you want to assign a LP. 
-	**BinCode**: Bin Code assigned to the product in the Warehouse Receipt.
-	**LocationCode**: Unit of measure assigned to the product in the Warehouse Receipt.
-	**ZoneCode**: Total number to receive expressed in the base unit of measure.

**Ouput**: Method that returns the number of assigned and pending LP to be assigned to a Warehouse Receipt.

-	**Created**: Boolean value that indicates if the process that was executed created a new License Plate. 
-	**LPPallet_DocumentNo**: Newly created LP Pallet number..


**Example**:

![image.png](/.attachments/image-44d8d90f-abb7-43c9-b0d4-9ec569e283d2.png)


**Request**:

    "jsonRequest":"{"ProcessMethod":"CreateLP_FromWarehouseReceiptLine","Parameters":[{"No":"107306","ItemNo":"1000","BinCode":"","UnitofMeasureCode":"PCS","TotalToReceive":"5","NoofPackLP":"1","PackUnitUoM":"PCS"}]}"

**Outputs**:

`"{"Created":true,"Message":"","LP_Pending_To_Receive":0,"LP_Received":"LP000281|LP000282"}"`

![image.png](/.attachments/image-8a2bd580-3e9f-444e-9429-2bd628f5dcf5.png)

**Note**: It is mandatory to have the check "Managed by Plur-E" marked on the Item Card in order to create LP and carry out movements through Warehouse Reclass Journal and Warehouse Item Journal.
![image.png](/.attachments/image-2938f245-9765-4198-97d8-43267217c1b2.png)

**Errors**:

```
{
  "Error": {
    "Code": "Configuration Error",
    "Message": "The item 1972-S is not managed by the Plur-e WMS module. If you want to configure it, you must go to the Item Card and turn on the check 'Managed by Plur-E'"
  }
}

{
  "Error": {
    "Code": "Not found",
    "Message": "The Warehouse Receipt Lines is empty
  }
}
```



