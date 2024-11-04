# **Plur-e Sales Manual**

## **1. INTRODUCTION**
Plur-E is a sales application integrated with Business Central

- Users must have:
  - Sales-related permissions in Business Central
  - Be listed in the Salespeople/Purchasers window

**IMPORTANT NOTES**

- All document types follow similar attachment and printing procedures
- Verification in Business Central is required for all transactions
- Payment batch configuration is essential for processing payments

------------

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

------------

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

**Picking Process**

Unlike partial shipment:

- Assign the full quantity for each item
- Verify that picking quantities match ordered quantities
- Don't split quantities as everything will be shipped together

**Final Validation**

- Check that all quantities are correct
- Confirm that the shipping location is appropriate
- Verify customer details
- Validate the order in Business Central

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

##**3. SALES RETURN ORDERS**

**Create New Return Order**

- Open Plur-e Mobile
- Navigate to "Sales Return Orders" section
- Click "Create New Return Order"
- Have original sales order reference ready

**Customer Selection**

- Search by:
  * Customer name/ID
  * Original order number
- Verify account status and eligibility
- Confirm shipping address

**Adding Items**

Manual Entry:
- Click "Add Return Item"
- Search by product code/name
- Select from original order

Scanning:
- Use device camera or Zebra scanner
- Scan product barcode
- Verify against original order

**4. Item Configuration**

For each item:
- Select return warehouse location
- Choose unit of measure (match original)
- Enter return quantity

**5. Business Central Validation**
- Review all return items
- Verify quantities and pricing
- Generate return authorization
- Process documentation
- Update inventory system


------------

## **4. SALES INVOICES**

**Creating New Sales Invoice**

Initial Access:
   - Open Plur-e Mobile application
   - Navigate to "Sales Invoices" section
   - Click "Create New Invoice" button
   - System opens new configuration tab

Initial Documentation:
   - Prepare customer order details
   - Gather pricing information
   - Check special discounts/promotions
   - Have tax information ready

**Customer Selection Process**

Customer Identification:
   - Search customer by:
     * Customer name
     * Customer ID
     * Account number
   - Verify customer account status
   - Confirm billing information

Account Verification:
   - Verify payment terms
   - Confirm billing address
   - Review special pricing agreements

**Adding Items to Invoice**

Manual Entry Method:
   - Click "Add Item" button
   - Search by:
     * Product code
     * Product name
     * Category
   - Select items from inventory
   - Verify pricing and availability

Scanning Function Method:
   - Access scanner function
     * Mobile device: Use camera
     * Zebra device: Use built-in scanner
   - Scan product barcode
   - Verify product details
   - Confirm pricing information

**Item Configuration Process**

Location Settings:
   - Select warehouse location
   - Verify stock availability
   - Choose shipping point
   - Confirm inventory levels

Unit of Measure Configuration:
   - Select appropriate unit
   - Verify pricing per unit
   - Check quantity breaks
   - Confirm volume discounts

Quantity Setup:

   - Enter ordered quantity
   - Verify against available stock
   - Check minimum order requirements
   - Calculate line total

Additional Item Details:

   - Apply any discounts
   - Add special pricing
   - Include item notes
   - Set tax codes

**5. Business Central Validation**

- Check that all quantities are correct
- Verify customer details
- Validate the invoice in Business Central

------------

## **5. SALES CREDIT MEMOS**

**Create New credit memo**

- Open Plur-e Mobile
- Navigate to "Sales credit memo" section
- Click "Create credit memo"
- Have original sales Invoice reference ready

**Customer Selection**

- Search by:
  * Customer name/ID
  * Original order number
- Verify account status and eligibility
- Confirm shipping address

**Adding Items**

Manual Entry:
- Click "Add Return Item"
- Search by product code/name
- Select from original order

Scanning:
- Use device camera or Zebra scanner
- Scan product barcode
- Verify against original order

**Item Configuration**

For each item:
- Select return warehouse location
- Choose unit of measure (match original)
- Enter return quantity

**5. Business Central Validation**

- Check that all quantities are correct
- Verify customer details
- Validate the invoice in Business Central


