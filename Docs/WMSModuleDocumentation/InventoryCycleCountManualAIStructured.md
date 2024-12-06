# **Inventory Cycle Count Guide**

This guide explains the procedures for performing an Inventory Cycle Count in a company using advanced Warehouse features within Business Central, as well as in the Plur-E application.

---

## **Table of Contents**
1. [Introduction](#1-introduction)
2. [Calculate Inventory by Specifications](#2-calculate-inventory-by-specifications)
   - [Initial Setup](#initial-setup)
   - [Configuration Steps](#configuration-steps)
   - [Processing](#processing)
3. [Calculate Inventory by Counting Period](#3-calculate-inventory-by-counting-period)
   - [Setup Counting Periods](#setup-counting-periods)
   - [Item Configuration](#item-configuration)
   - [Processing](#processing-1)
4. [Plur-E Inventory Cycle Count](#4-plur-e-inventory-cycle-count)
   - [Initial Setup](#initial-setup-1)
   - [Counting Process](#counting-process)
   - [Verification and Completion](#verification-and-completion)
5. [Important Notes and Best Practices](#important-notes-and-best-practices)

---

## **1. Introduction**

This manual provides step-by-step guidance on performing the Inventory Cycle Count using Business Central’s advanced Warehouse features. Business Central offers two main methods:
1. **Calculate Inventory by Specifications**
2. **Calculate Inventory by Counting Period**

---

## **2. Calculate Inventory by Specifications**

### **Initial Setup**

1. Open the **Physical Inventory Journals** page in Business Central.
2. Select or create a new **Batch**.
3. Click on **Calculate Inventory** to begin.

### **Configuration Steps**

1. Enter the **Document Number**.
2. Set filters:
   - **Filter by Item**:
     - General product posting group
     - Other specific filters as needed
   - **Filter Totals by**:
     - Location
     - Brand
     - Additional filtering options

### **Processing**

1. Review the updated **Physical Inventory Journals**.
2. For serialized products:
   - Use the **Clear Serials** option to reset serial quantities to zero before counting.

---

## **3. Calculate Inventory by Counting Period**

### **Setup Counting Periods**

1. Open the **Physical Inventory Counting Periods** page.
2. Create a new counting period:
   - Define the frequency (e.g., monthly, quarterly).
   - Enter any required information.

### **Item Configuration**

1. Access the **SKU** or **Items** page.
2. Define a **Physical Inventory Counting Period Code** for each item.
3. The system will automatically:
   - Assign the **Next Counting Start Date**.
   - Set the **End Date**.
   - Note: Dates can be adjusted manually if needed.

### **Processing**

1. Open the **Physical Inventory Journals** page.
2. Select or create a **Batch**.
3. Choose the **Calculate Counting Period** option.
4. Review products scheduled for counting on the selected posting date.
5. Enter the **Document Number**.
6. Confirm selections to proceed.

---

## **4. Plur-E Inventory Cycle Count**

### **Initial Setup**

1. Open the **Plur-E** application.
2. Select the relevant **Company**.
3. Access the **Inventory Cycle Count** module.

### **Counting Process**

1. Select the **Inventory Count** option.
2. Choose **Physical Inventory**.
3. Select the appropriate **Batch**.
4. Begin product scanning:
   - Scan the product label.
   - Enter the **Physical Quantity** for each product.
   - Use **Select Action → Edit** to adjust quantities if needed.

### **Verification and Completion**

1. Confirm sync with Business Central by checking for a confirmation message.
2. Verify line creation with the entered quantities in Business Central’s **Physical Inventory Journal**.
3. Repeat the process for each item in the inventory.
4. **Post the Journal** once all physical quantities have been entered.

---

## **5. Important Notes and Best Practices**

- **Filtering**: Use appropriate filters to avoid counting all products simultaneously.
- **Counting Period Customization**: Tailor counting periods to fit your business needs.
- **Data Synchronization**: Ensure all entries are synced between Plur-E and Business Central.
- **Pre-Posting Verification**: Always verify synced data before posting.
- **Manual Date Adjustments**: Counting dates can be manually modified if necessary.
- **Serialized Products**: Special handling is required for serialized products.
- **Batch Naming**: Use consistent naming conventions for batches.
- **Sync Status**: Regularly verify synchronization status.
- **Organized Schedules**: Maintain clear and organized counting schedules.
- **Documentation**: Document any manual adjustments for reference.
- **Data Backup**: Regularly back up counting data to prevent data loss.

---

This guide provides a structured process for efficient inventory cycle counting, supporting accuracy and effective synchronization with Business Central.
