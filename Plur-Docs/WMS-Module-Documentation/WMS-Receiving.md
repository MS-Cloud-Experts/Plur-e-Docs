# **WMS Receiving Module**

## **Overview**

The Warehouse Management System (WMS) Receiving Module in Business Central streamlines the process of receiving and handling incoming inventory. This module integrates with the PLUR-E mobile application to enhance efficiency in receiving, tracking, and storing items, including serialized and License Plate-managed items.

### **Contents**
1. [Receiving in Plur-e Mobile](#receiving-in-plur-e-mobile)
2. [Receiving in Business Central](#receiving-in-business-central)

---

## **1. Receiving in Plur-e Mobile**

The **Plur-e Mobile App** allows users to handle receiving tasks directly from their mobile devices, enabling easy tracking of items and inventory updates as items arrive at the warehouse.

### **Receiving Items**

1. **Access the Warehouse Receipt Section**:
   - Open the Warehouse Receipt section within the PLUR-E mobile app.
   - Ensure the user ID is assigned on the mobile device to display relevant orders.

2. **View and Select Orders**:
   - Enter the **Receipt** submodule to view created orders available for receiving.

3. **Select and Receive Items**:
   - Choose or scan the items to be received.
   - Enter the respective quantities for each item and confirm the data to update inventory.

### **Receiving Serialized Items**

1. **Serial Number Scanning**:
   - For serialized items, scan each serial number individually.
   - Record the quantity to maintain inventory accuracy and traceability.

2. **Verify Preloaded Serial Numbers**:
   - If the serial numbers are preloaded from an order, verify the data and proceed to confirm the receipt.

### **Put-Away Process (Location Assignment)**

Once items are received, users can initiate the **Put-Away Process** to assign a storage location within the warehouse.

1. **Initiate Put-Away**:
   - Decide whether to proceed with the put-away process immediately after receiving items.

2. **Assign Quantities and Locations**:
   - Enter the quantities to be stored in specific locations.
   - Select the destination Bin Code for each item, or apply location changes to all items in bulk.

---

## **2. Receiving in Business Central**

The **Business Central** interface allows users to manage and complete receipt tasks for items ordered via Purchase Orders.

1. **Create a Warehouse Receipt**:
   - After creating a **Purchase Order** in Business Central, select the **"Create Warehouse Receipt"** button.
   - This action generates a Warehouse Receipt document linked to the Purchase Order, where quantities can be received.

2. **Enter Quantities to Receive**:
   - Within the Warehouse Receipt document, fill in the quantities for each item in the **Qty to Receive** field.
   - **Note:** For items managed by the Plur-e system, receiving is done via **License Plate** functionalities within the app.

3. **Post the Receipt**:
   - Once quantities are recorded, post the Warehouse Receipt by clicking the **"Post Receipt"** button. This step finalizes the receiving process in Business Central, updating the inventory status for each received item.

