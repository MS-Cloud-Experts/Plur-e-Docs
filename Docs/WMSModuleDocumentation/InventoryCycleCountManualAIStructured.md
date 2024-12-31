# **Inventory Cycle Count Guide**

This guide explains the procedures for performing an Inventory Cycle Count in a company using advanced Warehouse features within Business Central, as well as in the Plur-E application.

## **1. Introduction**

This manual provides step-by-step guidance on performing the Inventory Cycle Count using Business Central’s advanced Warehouse features. Business Central offers two main methods:
1. **Calculate Inventory by Specifications**
3. **Calculate Inventory by Counting Period**

## **2. Calculate Inventory by Specifications**

![image](https://github.com/user-attachments/assets/6750e679-1e83-4f84-be2a-061e4978796f)

![image](https://github.com/user-attachments/assets/7842ba9f-8751-4c50-a0cb-0555b7fed814)

### **Initial Setup**

1. Open the **Physical Inventory Journals** page in Business Central.
2. Select or create a new **Batch**.
3. Click on **Calculate Inventory** to begin.

### **Configuration Steps**

1. Enter the **Document Number**.

 ![image](https://github.com/user-attachments/assets/24a74444-2772-45b9-802d-728a58d17127)
 
2. Set filters:
   - **Filter by Item**:
     - General product posting group
     - Other specific filters as needed
   - **Filter Totals by**:
     - Location
     - Brand
     - Additional filtering options

![image](https://github.com/user-attachments/assets/add61087-af1c-4e0b-9c17-4d2dc0591dc4)

### **Processing**

1. Review the updated **Physical Inventory Journals**.

![image](https://github.com/user-attachments/assets/3fc5f918-fbad-48b1-b8e7-bfd1607be912)

3. For serialized products:
   - Use the **Clear Serials** option to reset serial quantities to zero before counting.

![image](https://github.com/user-attachments/assets/e093182a-e905-4bb5-b7be-9dbe0e9e3d2b)

## **3. Calculate Inventory by Counting Period**

### **Setup Counting Periods**

1. Open the **Physical Inventory Counting Periods** page.

![image](https://github.com/user-attachments/assets/5beeb99a-5748-465b-986b-2f6d981cf448)

2. Create a new counting period:
   - Define the frequency (e.g., monthly, quarterly).
   - Enter any required information.
   - 
![image](https://github.com/user-attachments/assets/3f18b288-d4b4-44f2-9b85-2a3dd5982ee8)

### **Item Configuration**

1. Access the **SKU** or **Items** page.
2. Define a **Physical Inventory Counting Period Code** for each item.
3. The system will automatically:
   - Assign the **Next Counting Start Date**.
   - Set the **End Date**.
   - Note: Dates can be adjusted manually if needed.

![image](https://github.com/user-attachments/assets/883086cb-86a3-4c74-b9ab-a9746d9506f4)

### **Processing**

1. Open the **Physical Inventory Journals** page.

![image](https://github.com/user-attachments/assets/da557f3f-eb32-4b0c-8054-27e6c828a519)

2. Select or create a **Batch**.
3. Choose the **Calculate Counting Period** option.
4. Review products scheduled for counting on the selected posting date.
5. Enter the **Document Number**.

![image](https://github.com/user-attachments/assets/d0017b27-072c-438c-a8ad-2ad81effcaf6)

6. Confirm selections to proceed.

![image](https://github.com/user-attachments/assets/241d7698-46f6-4717-a9cf-f0efc9a0ab6b)

## **4. Plur-E Inventory Cycle Count**

### **Initial Setup**

1. Open the **Plur-E** application.
2. Select the relevant **Company**.
3. Access the **Inventory Cycle Count** module.

![image](https://github.com/user-attachments/assets/017e9a43-1211-4bab-a386-836954cfa268)

### **Counting Process**

1. Select the **Inventory Count** option.

![image](https://github.com/user-attachments/assets/f7a8b559-c096-4710-bdfd-41399054bb7e)

2. Choose **Physical Inventory**.

![image](https://github.com/user-attachments/assets/3b38afa4-3e60-4545-bbe4-7f700f2e5862)

3. Select the appropriate **Batch**.

![image](https://github.com/user-attachments/assets/10c83c02-af32-476b-8b8c-aafd87d0115b)

4. Begin product scanning:

![image](https://github.com/user-attachments/assets/55715b00-900f-4044-a88d-dba1f54ca36f)

   - Scan the product label.
   - Enter the **Physical Quantity** for each product.

![image](https://github.com/user-attachments/assets/b25e742b-9d4b-4b41-b8b9-af04896be70b)

   - Use **Select Action → Edit** to adjust quantities if needed.

![image](https://github.com/user-attachments/assets/90fa3f23-4e65-4909-b8bb-b04aa7831fe4)

![image](https://github.com/user-attachments/assets/c29feac1-34f7-4229-82df-778118dc0c3d)

![image](https://github.com/user-attachments/assets/52900bcb-b6a7-46d8-b778-8a5d47725de6)


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
