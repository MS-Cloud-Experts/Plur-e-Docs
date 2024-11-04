# **Plur-e Sales Manual**

This document provides a comprehensive guide for using the Plur-E sales application integrated with Business Central. It outlines procedures for managing sales orders, returns, invoices, and credit memos.

---

## **Table of Contents**
1. [Introduction](#1-introduction)
2. [Sales Orders](#2-sales-orders)
   - [Create Sales Order with Partial Shipment](#create-sales-order-with-partial-shipment)
   - [Create Sales Order with Complete Shipment](#create-sales-order-with-complete-shipment)
3. [Sales Return Orders](#3-sales-return-orders)
4. [Sales Invoices](#4-sales-invoices)
5. [Sales Credit Memos](#5-sales-credit-memos)

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

#### **2. Adding Items to the Order**
   - **Manual Entry**: Click on "Add Item" and search for the product by code or name.
   - **Scanning Function**: Click on the scan icon and use the camera to read the product barcode. Confirm the product before adding it.

#### **3. Item Configuration**
   - **Location Selection**: Choose the warehouse and verify availability.
   - **Unit of Measure**: Select the appropriate unit of measure.
   - **Quantity**: Enter the total quantity needed.

#### **4. Picking Process**
   - Set up the picking location and verify that quantities match the order.
   - Confirm the picking list and generate necessary documentation.

#### **5. Business Central Validation**
   - Verify that the quantities and shipping details are correct.
   - Approve the order in Business Central.

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

---

## **4. Sales Invoices**

### **Creating New Sales Invoice**
   - Open the Plur-e Mobile application and go to the "Sales Invoices" section.
   - Click on "Create New Invoice" and prepare the customer order details.

#### **Customer Selection Process**
   - Identify the customer by name, ID, or account number.
   - Verify the account status and billing information.

### **Adding Items to the Invoice**
   - **Manual Entry**: Click "Add Item" and search by code, name, or category.
   - **Scanning**: Use the scan function to read the product barcode.

#### **Item Configuration**
   - Select the warehouse location and verify stock availability.
   - Set up the unit of measure and ordered quantity.

#### **Business Central Validation**
   - Ensure that all quantities and customer details are correct.
   - Validate the invoice in Business Central.

---

## **5. Sales Credit Memos**

### **Create New Credit Memo**
   - Open Plur-e Mobile and navigate to the "Sales Credit Memo" section.
   - Click on "Create Credit Memo" and have the original sales invoice reference ready.

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

---

This manual provides a structured guide to managing orders, returns, invoices, and credit memos in the Plur-e application. The structure facilitates navigation and is suitable for training a chatbot AI.
