# Plur e Sales Manual

## 1. INTRODUCTION
Plur-E is a sales application integrated with Business Central

- Users must have:
  - Sales-related permissions in Business Central
  - Be listed in the Salespeople/Purchasers window

**IMPORTANT NOTES**

- All document types follow similar attachment and printing procedures
- Verification in Business Central is required for all transactions
- Payment batch configuration is essential for processing payments


## **2. SALES ORDERS**

###**Creating Sales Order with Partial Shipment**


**Create Sales Order in Plur-e Mobile**

- Access the Plur-e Mobile application
- Navigate to the "Sales Orders" section
- Click on "New Sales Order" button
- Select or verify the customer information
- Choose delivery address and billing details
- Set the desired delivery date

**Adding Items to the Order**

Manual Entry Method:

Click on "Add Item" or similar button

Search for products using:
- Product code
- Product name
- Select the desired item from the search results
- Verify product details before adding

Scanning Function Method

- Click on the scan button or barcode icon
- Position the camera to read the product barcode
- Verify that the scanned product is correct
- Confirm the addition to the order

**Item Configuration**

For each product in the order:

Location Selection:

- Choose the warehouse location
- Verify stock availability at selected location
- Confirm the picking location

Unit of Measure Settings:

- Select appropriate unit of measure
- Verify the conversion rates if applicable
- Confirm unit pricing

Quantity Configuration:

- Enter the total quantity needed
- Verify against available stock
- Confirm total amount matches customer request

**Picking Process**

Initial Setup:

- Access the picking function
- Verify order details
- Confirm picking location

Quantity Assignment:

- Assign full quantities for each item
- Verify stock availability
- Ensure picking quantities match order quantities

Picking Confirmation:

- Review all assigned quantities
- Confirm complete picking list
- Generate picking documentation

**Business Central Validation**

- Verify all quantities match
- Confirm complete shipment details
- Approve order in Business Central

###**Creating Sales Order with Complete Shipment**


**Starting the Order**

- Open Plur-e Mobile
- Go to the "Sales Orders" section
- Select "Create New Sales Order", the system will open a new tab where you can configure the new sales order.
- Adding Products

Manual Entry:

- Search for the product by name or code and select from the catalog

Scanning Function:
- Use the scanner to read barcodes, this scanner on a phone is the phone's camera, if it's a Zebra device it will come equipped with a barcode reader.
- Verify that the scanned product is correct

**Item Configuration**

For each product you must specify:

- Select the warehouse location
- Choose the correct unit of measure
- Enter the total quantity to be shipped
- Make sure the quantities match the available stock

Picking Process
Unlike partial shipment:

- Assign the full quantity for each item
- Verify that picking quantities match ordered quantities
- Don't split quantities as everything will be shipped together

Final Validation

- Check that all quantities are correct
- Confirm that the shipping location is appropriate
- Verify customer details
- Validate the order in Business Central

Shipment Confirmation

- Generate the shipping document
- Ensure all quantities are at 100%
- Confirm complete shipment

###**Key Differences with Partial Shipment and Recommendations**

- No need to split quantities
- All quantities must match the original order
- Picking is done in a single operation
- Validation is more straightforward as there's no need to control multiple shipments
- Verify available stock before creating the order
- Make sure all products are in the indicated location
- Confirm that you have shipping capacity for the entire order
- Document any incidents during the process

------------

## 3. SALES RETURN ORDERS
1. Create new return order
2. Select customer
3. Add items
4. For each item:
   - Select location
   - Choose unit of measure
   - Set quantity
5. Verify in Business Central

## 4. SALES INVOICES
1. Create new sales invoice
2. Select customer
3. Add items
4. For each item:
   - Select location
   - Choose unit of measure
   - Set quantity
5. Verify in Business Central

## 5. SALES CREDIT MEMOS
1. Create new credit memo
2. Select customer
3. Add items
4. For each item:
   - Select location
   - Choose unit of measure
   - Set quantity
5. Verify in Business Central

## 6. POST-CREATION OPERATIONS

6.1 Posting Documents
- Can post:
  - Sales orders
  - Return orders
  - Invoices
  - Credit memos

6.2 Posted Invoices
- View posted invoices
- Print posted invoices

