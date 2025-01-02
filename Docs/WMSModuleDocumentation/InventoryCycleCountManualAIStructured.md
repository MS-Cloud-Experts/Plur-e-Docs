# **Inventory Cycle Count Guide**

This guide explains the procedures for performing an Inventory Cycle Count in a company using advanced Warehouse features within Business Central, as well as in the Plur-E application.

## **1. Introduction**

This manual provides step-by-step guidance on performing the Inventory Cycle Count using Business Central’s advanced Warehouse features. Business Central offers two main methods:
1. **Calculate Inventory by Specifications**
3. **Calculate Inventory by Counting Period**

## **2. Calculate Inventory by Specifications**

![image](https://github.com/user-attachments/assets/2846ee68-1c2d-4e8e-849b-41a563fe30df)

![image](https://github.com/user-attachments/assets/72f47b03-8d52-43e2-974b-5024dc78406d)

### **Initial Setup**

1. Open the **Physical Inventory Journals** page in Business Central.
2. Select or create a new **Batch**.
3. Click on **Calculate Inventory** to begin.

### **Configuration Steps**

1. Enter the **Document Number**.

![image](https://github.com/user-attachments/assets/9ce325eb-d74d-45dc-aac9-5567cc98ed9b)

2. Set filters:
   - **Filter by Item**:
     - General product posting group
     - Other specific filters as needed
   - **Filter Totals by**:
     - Location
     - Brand
     - Additional filtering options

![image](https://github.com/user-attachments/assets/ecf6f12e-82a1-4b11-90dd-8af44b7c6e50)

### **Processing**

1. Review the updated **Physical Inventory Journals**.

![image](https://github.com/user-attachments/assets/a4cbf679-c446-4867-9df3-550fc9b95f59)

3. For serialized products:
   - Use the **Clear Serials** option to reset serial quantities to zero before counting.

![image](https://github.com/user-attachments/assets/46fe57ad-1047-4e16-93e1-a8c47c2f4599)

## **3. Calculate Inventory by Counting Period**

### **Setup Counting Periods**

1. Open the **Physical Inventory Counting Periods** page.

![image](https://github.com/user-attachments/assets/0523c2d4-4e8b-470b-ab1f-ff87f65308ca)

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
 
![image](https://github.com/user-attachments/assets/78d96565-ac10-4145-b46c-f359201faad9)



### **Processing**

1. Open the **Physical Inventory Journals** page.

![image](https://github.com/user-attachments/assets/1fff9b44-8fed-4f18-9c09-945a3c1c3363)

2. Select or create a **Batch**.
3. Choose the **Calculate Counting Period** option.
4. Review products scheduled for counting on the selected posting date.
5. Enter the **Document Number**.

![image](https://github.com/user-attachments/assets/ae635893-bb25-4f4d-be63-42c6668c5c27)

6. Confirm selections to proceed.

![image](https://github.com/user-attachments/assets/82f64308-ea6d-4958-8ec1-250d23fffc9a)

---

## **4. Plur-E Inventory Cycle Count**

### **Initial Setup**

1. Open the **Plur-E** application.
2. Select the relevant **Company**.
3. Access the **Inventory Cycle Count** module.

![image](https://github.com/user-attachments/assets/38902992-c544-40f5-ab82-666a75b5cd1e)

### **Counting Process**

1. Select the **Inventory Count** option.

![image](https://github.com/user-attachments/assets/f8017b51-8f74-4361-9d43-1b5c40a66e47)

2. Choose **Physical Inventory**.

![image](https://github.com/user-attachments/assets/2324241f-b821-49f8-b17d-d7899d982127)

3. Select the appropriate **Batch**.

![image](https://github.com/user-attachments/assets/d5a09a06-a6cb-4886-bf2b-46d13d8a8562)

4. Begin product scanning:

   - Scan the product label.
   - Enter the **Physical Quantity** for each product.

![image](https://github.com/user-attachments/assets/0ffd6d01-e9fe-4fc2-b1e8-59b0d8f47740)

   - Use **Select Action → Edit** to adjust quantities if needed.

![image](https://github.com/user-attachments/assets/49be5bc5-f96b-4ddd-877e-89abbaaf03f0)

![image](https://github.com/user-attachments/assets/70d5c202-6e4f-49bf-beaa-d8b39a35b638)

![image](https://github.com/user-attachments/assets/6bbd714b-bbe2-444a-99fe-4f8025a41879)


### **Verification and Completion**

1. Confirm sync with Business Central by checking for a confirmation message.
2. Verify line creation with the entered quantities in Business Central’s **Physical Inventory Journal**.
3. Repeat the process for each item in the inventory.
4. **Post the Journal** once all physical quantities have been entered.


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

# **Video** 
[![Video explicativo](https://img.youtube.com/vi/UtU60Vq-vPw/0.jpg)](https://youtu.be/UtU60Vq-vPw?si=YGzuT7zVd6Y48EeB)


This guide provides a structured process for efficient inventory cycle counting, supporting accuracy and effective synchronization with Business Central.
