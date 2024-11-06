# **Sales Module in Business Central**

## **Overview**

The Sales Module in Business Central enables businesses to manage and record sales transactions, handle agreements with customers, record completed sales, manage returns, and make corrections. The module includes key documents: **Sales Orders**, **Sales Invoices**, **Sales Return Orders**, and **Sales Credit Memos**. Each document serves a distinct purpose to ensure accuracy and efficiency in the sales process.

---

## **1. Sales Orders**

Sales Orders are used to record an agreement to sell specific products or services under agreed delivery and payment terms.

### **Steps to Create and Manage a Sales Order**

1. **Create a Sales Quote (Optional)**:
   - Start by creating a **Sales Quote** to outline terms and pricing for the customer’s review.
   - Convert the quote to a **Sales Order** or **Sales Invoice** if the customer agrees to proceed.

2. **Create a Sales Order**:
   - Access the **Sales Orders** page and select **New** to create a new order.
   - Enter **Customer Information** including name, address, payment terms, and delivery terms.

3. **Enter Sales Order Lines**:
   - Add each product or service in the **Lines** section with details such as **Item Number**, **Quantity**, **Price**, and **Discounts**.

4. **Order Promising and Delivery Dates**:
   - Use the **Order Promising** feature to set and communicate realistic delivery dates based on inventory and delivery schedules.

5. **Send an Order Confirmation**:
   - Send an **Order Confirmation** to the customer after they confirm the order.

6. **Partial Shipments or Drop Shipments**:
   - For partial shipments, update the **Quantity Shipped** field for each partial delivery.
   - If using drop shipment, specify the supplier and delivery details for direct shipment from the supplier.

7. **Posting the Sales Order**:
   - Post the **Sales Order** to create a **Sales Invoice** and record the transaction.

8. **Correct or Cancel Sales Order**:
   - If unpaid, correct or cancel the posted invoice if adjustments are needed.
   - If paid, create a **Sales Credit Memo** to process adjustments.

---

## **2. Sales Invoice**

Sales Invoices finalize the sale agreement, recording the sale of goods or services and updating inventory and financial records.

### **Steps to Create and Manage a Sales Invoice**

1. **Generate a Sales Invoice from a Sales Order**:
   - Convert a **Sales Order** directly into a Sales Invoice to maintain consistency.

2. **Create a New Sales Invoice**:
   - Access the **Sales Invoices** page and select **New**.
   - Enter **Customer Information** along with payment and delivery terms.

3. **Enter Sales Invoice Lines**:
   - Add each item or service, specifying quantities, prices, and applicable discounts.

4. **Post the Sales Invoice**:
   - Post the invoice to update the general ledger and inventory records.

5. **Correcting or Cancelling a Sales Invoice**:
   - For unpaid invoices, **Cancel** or **Correct** errors.
   - For paid invoices, create a **Sales Credit Memo** to adjust the records as needed.

---

## **3. Sales Return Order**

Sales Return Orders are created to process items returned by customers, updating inventory and financial records accordingly.

### **Steps to Create and Manage a Sales Return Order**

1. **Create a Sales Return Order**:
   - Access the **Sales Return Orders** page and select **New**.
   - Enter customer details and any return conditions on the **General FastTab**.

2. **Copy Information from Original Documents**:
   - Use the **Copy Document** function to pull details from the original Sales Invoice or Sales Order.

3. **Enter Return Order Lines**:
   - Add each returned item, including original quantities, prices, and reasons for the return.

4. **Process and Post the Return**:
   - Verify the return details and post the order, updating inventory and financial records.

---

## **4. Sales Credit Memo**

Sales Credit Memos reverse or adjust previously posted sales transactions, especially for unpaid invoices or correcting errors.

### **Steps to Create and Manage a Sales Credit Memo**

1. **Create a Credit Memo from an Unpaid Invoice**:
   - Locate the unpaid Sales Invoice to be reversed.
   - Use the **Create Credit Memo** function to generate a credit memo linked to the invoice.

2. **Enter Credit Memo Details**:
   - Adjust information on the **Sales Credit Memo** page to reflect the correction.

3. **Recreate or Cancel the Original Invoice**:
   - Decide whether to **Cancel** the original invoice or **Recreate** it with the corrected information.

4. **Post the Credit Memo**:
   - Post the credit memo to update financial records, reflecting the reversal or correction.

---

## **Summary of Document Functions**

| Document              | Purpose                                                                                 | Key Features                                    |
|-----------------------|-----------------------------------------------------------------------------------------|-------------------------------------------------|
| **Sales Order**       | Record agreements with customers, including delivery and payment terms.                 | Allows partial shipments, order promising.      |
| **Sales Invoice**     | Officially records a sale and updates general ledger and inventory.                     | Correct or cancel before payment is received.   |
| **Sales Return Order**| Records customer returns and adjusts inventory and financial records.                   | Copy from original documents for accuracy.      |
| **Sales Credit Memo** | Reverses or corrects transactions, especially for unpaid or erroneous invoices.         | Cancels or recreates original invoices.         |


