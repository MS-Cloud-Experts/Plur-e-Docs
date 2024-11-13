# Warehouse Shipment Process Guide

## Overview
This guide details the step-by-step process for creating and processing a warehouse shipment in the Business Manager system.

## Prerequisites
- Access to Business Manager Role Center
- Appropriate permissions for Sales Orders and Warehouse operations

## Step-by-Step Process

### 1. Creating a Sales Order
1. Navigate to Business Manager Role Center
2. Access Sales Orders
3. Click "New" to create a new Sales Order
4. Enter customer information:
   - Select customer using the lookup function
   - Choose appropriate customer from the list

### 2. Adding Items to Sales Order
1. In the Sales Lines section:
   - Click the lookup function in the "No." field
   - Select the desired item from the list
2. Enter item details:
   - Set quantity to required amount (in this case: 100)
   - Select Location Code using the lookup function

### 3. Creating Warehouse Shipment
1. Click "Create Warehouse Shipment"
2. System confirms creation with message: "1 Warehouse Shipment Header has been created"
3. The Warehouse Shipment document opens (Example: WHSE SHIP-00011)

### 4. Assigning Warehouse Employee
1. Click lookup function in "Assigned User ID" field
2. Select appropriate warehouse employee from the list

### 5. Creating Pick Document
1. Click "Create Pick"
2. Confirm in the "Whse.-Shipment - Create Pick" dialog
3. System generates pick document (Example: WHSE PICK-00008)

### 6. Processing Pick Lines
1. Click "Pick Lines" to view Warehouse Pick Lines
2. Click "Show Document" to view full pick document
3. Assign License Plates:
   - Click "Assign License Plates to Warehouse Pick"
   - Select appropriate license plate from the list (Example: LP-00013)
   - System confirms successful assignment

### 7. Registering and Posting Pick
1. Click "Register Pick"
2. Confirm the registration when prompted
3. Close the Warehouse Pick document

### 8. Posting Shipment
1. Click "Post Shipment"
2. Confirm posting in the dialog
3. System confirms successful posting with message:
   ```
   Number of source documents posted: 1 out of a total of 1.
   Ship lines have been posted.
   ```

## Important Documents Generated
- Sales Order (New)
- Warehouse Shipment (WHSE SHIP-00011)
- Warehouse Pick (WHSE PICK-00008)
- License Plate Assignment (LP-00013)

## Notes
- All steps require proper verification before proceeding
- System generates confirmation messages at key points
- Document numbers may vary but follow similar format
- Always ensure proper assignment of warehouse employees and license plates

[Recording_Shiptment_full.txt](/.attachments/Recording_Shiptment_full-16f55bda-61c4-4b4e-bd15-4b69c2aa15a0.txt)
