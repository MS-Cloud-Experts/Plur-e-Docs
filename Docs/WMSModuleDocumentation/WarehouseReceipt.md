# **INTRODUCTION**
The Plur-e mobile app transforms warehouse receiving processes by providing a comprehensive, user-friendly solution for inventory management that seamlessly integrates with Business Central. Designed to streamline item receipt, tracking, and verification, this innovative mobile application empowers warehouse professionals to manage incoming inventory with unprecedented precision, efficiency, and ease. By offering advanced features such as real-time serial number scanning, tracking configuration review, and instant synchronization with Business Central, Plur-e revolutionizes traditional receiving workflows, reducing manual errors and significantly improving overall warehouse operational effectiveness.

# **RECEIVING PROCESS WITH PLUR-E MOBILE APP**

## **Receiving Items**

## **Initiating the Receipt Process**

Open the Warehouse Receipt (Wshe receipt) section on the Plur-e app.

![image](https://github.com/user-attachments/assets/83b6d64b-09ec-46a0-b99a-c5b99f9ec28e)

![image](https://github.com/user-attachments/assets/be3bbe7b-3595-4531-823b-5682a9036658)

## **Accessing the Warehouse Receipt Submodule**

On the device, enter the submodule to view the created receipt.

![image](https://github.com/user-attachments/assets/6055ae0b-80d2-4b48-a3a9-dc8d9bbb7afe)

## **Selecting Items for Receipt**

Select or scan the item to be received, starting with one without tracking.

Enter the quantities and press the send button.

![image](https://github.com/user-attachments/assets/f40dd582-98fa-4508-9f1f-6e7f78301781)

## **Receiving Serialized Items**

Repeat the process for a serialized item, including checking the tracking configuration if necessary.

Scan the serial numbers individually, with options for counting and deleting if required.

![image](https://github.com/user-attachments/assets/e1876435-60bc-4dc5-96b4-ebefeb0ca0ea)

## **Entering Received Quantities**

Begin by inputting the quantities of items you are receiving. This step is crucial for inventory accuracy and ensures that the system reflects the actual number of items entering your warehouse.

![image](https://github.com/user-attachments/assets/01b7bd74-3f6d-49b4-b0d1-dc40cc73c803)

![image](https://github.com/user-attachments/assets/a69194cb-f13f-4558-96f8-2a47700ea5a8)

## **Accessing Tracking Configuration**

- ## **Understanding Tracking Configuration**

If you need to review or understand the item tracking configuration, simply click on the interrogation sign icon. This action provides access to detailed tracking settings for the items, offering clarity on how each item is monitored within the system.

![image](https://github.com/user-attachments/assets/c5045625-c571-4d64-afe0-794dde4e592c)

## **Scanning Serial Numbers**

- ## **Scanning Serial Numbers Individually**

Proceed to scan the serial numbers of the received items one by one. This step is essential for tracking individual items, especially for those that require serialization for inventory management and traceability.

![image](https://github.com/user-attachments/assets/0b62e0c3-b4de-4e5a-b4f7-2b692dcc70e9)

- ## **Actions Upon Scanning Serials**

Each scan of a serial number allows for two actions: firstly, it counts each serial number, ensuring accuracy in quantity; secondly, it provides visibility for each scanned serial, enhancing traceability and verification.

![image](https://github.com/user-attachments/assets/67cdd261-799a-44ca-8af7-587959785e50)

- ## **Selection and Deletion Option**

As serial numbers are scanned, you'll have the option to select and, if necessary, delete any serial number. This feature is particularly useful for correcting any errors during the scanning process, ensuring that only the correct items are recorded.

![image](https://github.com/user-attachments/assets/deb48090-d7e3-4309-ac59-b0e9d1dd6bd4)

- ## **Sending Serial Numbers to Business Central (BC)**

Upon completing the count and verification of serial numbers, the "send" option becomes available. Selecting this will transmit the serial number data to Business Central, finalizing the creation and recording of serials in your inventory system.

![image](https://github.com/user-attachments/assets/2d7ded5c-4d06-4b5f-918e-cc67efb7a4b1)

![image](https://github.com/user-attachments/assets/104db79e-39c2-4434-ad7e-bf1732fde62e)

- ## **Handling Preloaded Serials from Orders**

If serial numbers are preloaded from a transfer order or purchase order, there's no need to scan them again. You will have the option to simply view the preloaded serials. This feature ensures efficiency and accuracy in inventory management by reducing manual scanning efforts.

![image](https://github.com/user-attachments/assets/56a08417-ed2c-4bfb-8e3e-8973a00d91ce)

![image](https://github.com/user-attachments/assets/c503dd8b-7d36-4208-bb9a-d1fa242854ba)

- ## **Posting Option upon Completion**

Upon finalizing the receipt or pick process, you'll find a posting option at the bottom of the screen. This allows you to finalize the transaction in the system, indicating that the items are ready for the next phase in the workflow.

![image](https://github.com/user-attachments/assets/0b024873-64d5-4c08-b226-55f6dff17447)

# **SUMMARY**

## **Overview**

The Warehouse Management System (WMS) Receiving Module in Business Central streamlines the process of receiving and handling incoming inventory. This module integrates with the PLUR-E mobile application to enhance efficiency in receiving, tracking, and storing items, including serialized and License Plate-managed items.

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



