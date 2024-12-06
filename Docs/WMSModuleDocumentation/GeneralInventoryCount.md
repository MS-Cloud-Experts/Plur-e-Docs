# GENERAL INVENTORY COUNT MANUAL

## 1. INTRODUCTION

- Manual designed to explain the procedure to perform the General Inventory Count in a company that doesn't use advanced Warehouse
- This option allows counting inventory items without previously loading them in a Batch
- The procedure is performed using the Plur-E application

## 2. PLUR-E GENERAL INVENTORY COUNT

### Initial Setup

1. Open Plur-E application
2. Verify correct company selection
3. Access Inventory Cycle Count module

### Location Configuration

1. Verify correct location is selected
   - Note: Default location is set in user preferences in Plur-E Web
2. Select General Inventory Count option
3. Choose Physical Inventory

### Batch Selection

1. Select corresponding Batch for count information storage
2. Important: Information in Business Central Batch will be overwritten by Plur-E data

### Counting Process

1. Access product scanning page
![Media (51).jpg](/.attachments/Media%20(51)-bc1a0b50-7bc7-424d-80fe-0c9dfca0416e.jpg)
2. For each item:
   - Scan product label
   - Enter physical quantity
   - System will process based on three scenarios:
     - **Scenario 1:** Physical quantity less than calculated quantity
       * Generates negative adjustment in Physical Inventory Journal
     - **Scenario 2:** New item or zero calculated quantities
       * Generates positive adjustment in Physical Inventory Journal
     - **Scenario 3:** Physical quantity greater than calculated quantity
       * Generates positive adjustment in Physical Inventory Journal

### Verification and Completion

1. Select "Finish" option after counting all items
2. Check confirmation message for Business Central sync
3. Verify line creation in Business Central's Physical Inventory Journal
4. Post Journal after verification

## IMPORTANT NOTES AND BEST PRACTICES

- Always verify company selection before starting
- Ensure correct location is selected
- Understand that Batch data will be overwritten
- Verify synced data before posting
- Maintain organized counting process
- Document any discrepancies
- Regular verification of sync status
- Check all adjustments before posting