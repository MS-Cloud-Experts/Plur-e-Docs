# Plur-E Installation and Configuration Manual V2

## Introduction
Plur-E is a mobile application for Android devices that provides fast and efficient management of the sales, warehouse, inventory management, and payment modules of Dynamics 365 Business Central ERP through its extension.

## Prerequisites to install the Plur-E extension in Business Central
The following prerequisites are needed to install and configure the Plur-E extension, as well as how to configure the Plur-E web command and control center:

1. Dynamics 365 Business Central production environment or Sandbox to install the extension.
2. Global administrator user of all the companies configured in Business Central.
3. Android device on which Plur-E Mobile will be installed.

Note: See Appendix A for how to set global administrator permissions on a Dynamics 365 Business Central user.

## Installation of the Plur-E extension in Business Central
1. Search for the Plur-E extension for Business Central in Microsoft AppSource.

![image](https://github.com/user-attachments/assets/c6cabfc7-cb1d-4809-a709-a35f3c34b49e)

3. Enter the account from which you want to acquire the extension (remember to have a user with global administrator permissions for an efficient installation and configuration).

![image](https://github.com/user-attachments/assets/c2b33aea-8cb4-4ef1-99a1-f5c71925a61c)

5. Select the environment in which the extension will be installed.

![image](https://github.com/user-attachments/assets/b6d6f45e-5906-4277-a8ac-abbfc975c982)

7. Follow the steps given by Business Central to install the Plur-E extension.

![image](https://github.com/user-attachments/assets/c2c53716-dedb-440c-a547-b7068489d1ec)

Note: Keep in mind that, when installing an extension, Business Central will interrupt the sessions of all users who are using the environment.

5. Once the Plur-E extension is installed, go to the Business Central page called Assisted Setup and select Plur-E Setup to open the Plur-E Wizard and configure it.

![image](https://github.com/user-attachments/assets/907fad12-19a2-49a4-bc3d-f15c9138ca6d)

7. Follow the terms and conditions in the Plur-E Wizard.

![image](https://github.com/user-attachments/assets/c4fd32e2-1a54-4047-ba8e-5fc3875e7844)
   
9. The next step will open the Azure Active Directory application of Business Central that will allow you to grant the necessary permissions to Plur-E. Within the window that appears next, click on "Grant Consent".

![image](https://github.com/user-attachments/assets/f3b3a077-ca4e-495c-81fc-1699dc7f468e)

11. Once the extension is activated, the wizard will allow you to configure the document series that Plur-E can use in the Mobile Application. This list of series will be "Pre-selected" according to the modules purchased on the Plur-E portal.

![image](https://github.com/user-attachments/assets/dd5eca2c-9294-474b-9a53-3d37da5e9b90)

13. By clicking the "Next" button, you have finished configuring the Plur-E extension.

![image](https://github.com/user-attachments/assets/f56094b3-0f19-4e1e-8f1c-7e9d1aaacfac)

15. If you search in the Business Central search engine for the Plur-E Setup page, you will see all the settings and the link to the Plur-E web administration portal, where you can configure the modules you have subscribed and configured, for example, the Sales Module.

![image](https://github.com/user-attachments/assets/e1257b95-ba85-45e3-a4ce-7ef129e011dd)

![image](https://github.com/user-attachments/assets/472f2951-ab93-425c-a21f-9bd9989e9086)


## Other aspects to consider during installation
### Aspect 1
If you get the following message: "Go to the central business Extensions Manager page and select the Plur-E extension and select the configure option."

![image](https://github.com/user-attachments/assets/178d71f4-0bf9-4970-85b1-7bd9ecdccccf)

![image](https://github.com/user-attachments/assets/dfb91be7-94eb-41e1-86a2-c116fc52c8f2)

1. Once in this section, you must activate the check called "Allow HttpClient Requests".

![image](https://github.com/user-attachments/assets/ec48245c-629e-485e-ad47-73d492a9616a)

### Aspect 2
Once the installation of the Plur-E extension is finished, the users and environments must be configured in the Plur-E web portal.
1. In the Environments section of the Plur-E web portal, you can configure the Business Central environments that have the Plur-E extension installed and configured.
2. In the Users section, you can configure the users that will use the mobile application by configuring their subscriptions and available environments.
3. Once the users have been created, they will receive a temporary password to enter the mobile application. Once inside the application, the password can be changed for the convenience of the user who is using it.

## Appendices
### Appendix A
In this appendix, you will find the way to configure a central business user with global administrator permissions.
1. Go to the following link: https://portal.office.com/Adminportal/Home#/users
3. Select the user to which you want to give global permissions.

![image](https://github.com/user-attachments/assets/71e451aa-e8dc-488f-9d3b-7411e027b01a)

5. Select the "Manage Roles" option.

![image](https://github.com/user-attachments/assets/30701fbb-3496-41b0-94a6-1d3cfddb9fbc)

6. Check the "Admin Center Access" and then "Global Administrator" options.

![image](https://github.com/user-attachments/assets/512d34fd-cc3d-4869-960c-a7e6fabb8331)

It is also recommended to configure the user who is going to install the extension as "Super" in Business Central.

![image](https://github.com/user-attachments/assets/51272e36-0a23-4fe5-9136-dd03797f7a9a)
