# **Plur-e Sales Manual**

This document provides a comprehensive guide for using the Plur-E sales application integrated with Business Central. It outlines procedures for managing sales orders, returns, invoices, and credit memos.

---

## **1. Introduction**

Plur-E is a sales application integrated with Business Central.

### **User Requirements**
- Users must have:
  - Sales-related permissions in Business Central.
  - Be listed in the Salespeople/Purchasers window.

### **Important Notes**
- All document types follow similar attachment and printing procedures.
- Verification in Business Central is required for each transaction.
- Payment batch configuration is essential for processing payments.

![image](https://github.com/user-attachments/assets/06914287-2f70-42a4-90ce-869f2a013886)

---

## **2. Sales Orders**

### **Create Sales Order with Partial Shipment**

#### **1. Create Sales Order in Plur-e Mobile**
   - Open the Plur-e Mobile application.
   - Go to the "Sales Orders" section.
   - Click on "New Sales Order".
   - Select or verify the customer information.
   - Choose the delivery address and billing details.
   - Set the desired delivery date.

![image](https://github.com/user-attachments/assets/ac9040bb-66ba-4662-acd1-5dd55d245872)

![image](https://github.com/user-attachments/assets/45123121-c94b-489c-b25c-2df20fa2e667)

#### **2. Adding Items to the Order**
   - **Manual Entry**: Click on "Add Item" and search for the product by code or name.
   - **Scanning Function**: Click on the scan icon and use the camera to read the product barcode. Confirm the product before adding it.

![image](https://github.com/user-attachments/assets/1f587c2d-6888-47c8-8198-28dbea9e3dbf)

![image](https://github.com/user-attachments/assets/f83f6cbf-03a8-48ed-9045-0eb30fcb0810)

#### **3. Item Configuration**
   - **Location Selection**: Choose the warehouse and verify availability.
   - **Unit of Measure**: Select the appropriate unit of measure.
   - **Quantity**: Enter the total quantity needed.

![image](https://github.com/user-attachments/assets/a222df95-bc78-47aa-8051-c089f900bde5)

#### **4. Picking Process**
   - Set up the picking location and verify that quantities match the order.
   - Confirm the picking list and generate necessary documentation.

#### **5. Business Central Validation**
   - Verify that the quantities and shipping details are correct.
   - Approve the order in Business Central.

![image](https://github.com/user-attachments/assets/31b5a624-2e0d-4c58-b323-909b088dc4b3)

![image](https://github.com/user-attachments/assets/bfea7e52-5c85-45c7-8000-5f3619de61e7)

---

### **Create Sales Order with Complete Shipment**

#### **1. Start the Order**
   - Open Plur-e Mobile, go to "Sales Orders", and select "Create New Sales Order".
   - Configure order information in the new tab.

#### **2. Adding Products**
   - **Manual Entry**: Search for the product and select it from the catalog.
   - **Scanning**: Use the camera or Zebra scanner to read barcodes.

#### **3. Item Configuration**
   - Specify the warehouse location, unit of measure, and total quantity to be shipped.

#### **4. Picking Process**
   - Assign the full quantity for each item. No quantity splits are needed as everything will be shipped together.

#### **5. Final Validation**
   - Ensure all quantities are correct and confirm the shipping location.
   - Validate the order in Business Central.

---

### **Key Differences with Partial Shipment and Recommendations**
   - In complete shipment, no quantity splitting is needed.
   - All picking is done in a single operation.
   - Verify available stock before creating the order and ensure shipping capacity for the entire order.

---

## **3. Sales Return Orders**

### **Create New Return Order**
   - Open Plur-e Mobile and navigate to the "Sales Return Orders" section.
   - Click on "Create New Return Order" and have the original sales order reference ready.

![image](https://github.com/user-attachments/assets/296cf05e-6213-41b7-a4fb-a7fc7f4a8fdf)

![image](https://github.com/user-attachments/assets/2844efec-a572-40b1-9839-0c4fb8d30288)

### **Customer Selection**
   - Search by customer name or original order number.
   - Verify account status and shipping address.

### **Adding Items**
   - **Manual Entry**: Click "Add Return Item" and select from the original order.
   - **Scanning**: Use the camera or Zebra scanner to read the product barcode.

#### **Item Configuration**
   - Select the return warehouse location, unit of measure, and return quantity.

#### **Business Central Validation**
   - Review return items and quantities.
   - Generate return authorization and update the inventory system.

![image](https://github.com/user-attachments/assets/55293b76-cf92-449b-bebc-ace9cece6e12)

---

## **4. Sales Invoices**

### **Creating New Sales Invoice**
   - Open the Plur-e Mobile application and go to the "Sales Invoices" section.
   - Click on "Create New Invoice" and prepare the customer order details.

![image](https://github.com/user-attachments/assets/6e00bec5-888f-4f91-8869-343df8c2bd3c)

![image](https://github.com/user-attachments/assets/a5df97d4-6875-4404-ba96-aa6570248e78)

#### **Customer Selection Process**
   - Identify the customer by name, ID, or account number.
   - Verify the account status and billing information.
   - 
### **Adding Items to the Invoice**
   - **Manual Entry**: Click "Add Item" and search by code, name, or category.
   - **Scanning**: Use the scan function to read the product barcode.

#### **Item Configuration**
   - Select the warehouse location and verify stock availability.
   - Set up the unit of measure and ordered quantity.

#### **Business Central Validation**
   - Ensure that all quantities and customer details are correct.
   - Validate the invoice in Business Central.

![image](https://github.com/user-attachments/assets/00206d0e-0a36-415c-90b5-4e01b83db70c)

---

## **5. Sales Credit Memos**

### **Create New Credit Memo**
   - Open Plur-e Mobile and navigate to the "Sales Credit Memo" section.
   - Click on "Create Credit Memo" and have the original sales invoice reference ready.

![image](https://github.com/user-attachments/assets/cb1083eb-9e42-4206-b7b8-f58a9440e45d)

![image](https://github.com/user-attachments/assets/fe922c91-e91a-42b8-b975-4d21342ee27e)

### **Customer Selection**
   - Search by customer name or original order number.
   - Verify account status and shipping address.

### **Adding Items**
   - **Manual Entry**: Click "Add Return Item" and select from the original order.
   - **Scanning**: Use the camera or Zebra scanner to read the product barcode.

#### **Item Configuration**
   - Select the return warehouse location, unit of measure, and return quantity.

#### **Business Central Validation**
   - Review that all quantities and customer details are correct.
   - Validate the credit memo in Business Central.

![image](https://github.com/user-attachments/assets/3f7bec84-5a95-4a43-a693-9ed112eb0cde)

---

This manual provides a structured guide to managing orders, returns, invoices, and credit memos in the Plur-e application. The structure facilitates navigation and is suitable for training a chatbot AI.
