# Configuring Payment Methods in **Plur-e** on **Business Central**

To set up payment methods for the **Plur-e** application in **Business Central**, follow these steps:

## 1. Setting Up the **General Journal Template**

- Go to the **General Journal Template** page in **Business Central**.
- Create a new template named **Payments**.
- After creating the template, create **batches** to represent the payment methods for the **Plur-e** application.

## 2. Creating **General Journal Batches**

- In the **General Journal Template** page, select the **Payments** template.
- Click on the **Batches** button at the top of the page to open the batch setup for this template.
- Create the necessary **batches**, filling in the following key fields:
  - **Name**: Specify the name of the batch.
  - **Bal. Account Type**: Set the type for the balancing account.
  - **Bal. Account No.**: Enter the account number for balancing.
  - **Payment Method Code**: Define the code for the payment method.

- After setting up and configuring these fields, access the **Plur-e Dashboard** and create the same payment methods. *(Note: For more information, refer to the **Plur-e Dashboard Manual**).*

## Key Points

- The **General Journal Template** is where you create the **"Payments"** template.
- The **General Journal Batches** are where you configure the individual payment methods, including the **name**, **balance account type**, **balance account number**, and **payment method code**.
- The payment methods configured in **Business Central** need to be replicated in the **Plur-e Dashboard** for them to be available in the **mobile application**.
