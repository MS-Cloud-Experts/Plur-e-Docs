#INVENTORY CYCLE COUNT MANUAL

##1. INTRODUCTION
- Manual designed for Adventure Sports Retail's Inventory Cycle Count
- Two main methods available in Business Central:
  1. Calculate Inventory by Specifications
  2. Calculate Inventory by Counting Period

##2. CALCULATE INVENTORY BY SPECIFICATIONS

**Initial Setup**

1. Open Physical Inventory Journals page
2. Select or create new Batch
3. Choose "Calculate Inventory" option

**Configuration Steps**

1. Enter document number
2. Set filters:
   - Filter Item section:
     * General product posting group
     * Other specific filters
   - Filter totals by section:
     * Location
     * Brand
     * Other filtering options

**Processing**
1. Review updated Physical Inventory Journals
2. For serialized products:
   - Use "Clear Serials" option to initialize serials to zero

##3. CALCULATE INVENTORY BY COUNTING PERIOD

**Setup Counting Periods**
1. Open Physical Inventory Counting Periods page
2. Create new period:
   - Define frequency (e.g., monthly, quarterly)
   - Set required information

**Item Configuration**
1. Access SKU or items page
2. Define Physical Inventory Counting Period Code for items
3. System will:
   - Assign Next Counting Start Date
   - Set End Date
   - Note: Dates can be manually adjusted

**Processing**
1. Open Physical Inventory Journals
2. Select/create Batch
3. Choose "Calculate Counting Period" option
4. Review products due for counting on selected posting date
5. Enter document number
6. Confirm selections

##4. PLUR-E INVENTORY CYCLE COUNT

**Initial Setup**
1. Open Plur-E application
2. Select Adventure Sports retail company
3. Access Inventory Cycle Count module

**Counting Process**
1. Select Inventory Count option
2. Choose Physical Inventory
3. Select appropriate Batch
4. Perform product scanning:
   a. Scan product label
   b. Enter physical quantity
   c. Use Select Action → Add option
   d. Confirm with ADD icon

**Verification and Completion**
1. Check confirmation message for Business Central sync
2. Verify line creation with entered amount
3. Confirm update in Business Central's Physical Inventory Journal
4. Repeat process for each item
5. Post Journal after all physical quantities are entered

##IMPORTANT NOTES AND BEST PRACTICES

- Cannot count all products simultaneously - use appropriate filters
- Counting periods can be customized to business needs
- All entries sync between Plur-E and Business Central
- Always verify synced data before posting
- Manual adjustments of counting dates are possible
- Serialized products require special handling
- Use consistent naming conventions for batches
- Regularly verify sync status
- maintain organized counting schedules
- Document any manual adjustments
- Regular backup of counting data
