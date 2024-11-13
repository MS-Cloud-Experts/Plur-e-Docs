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
2. Enter the account from which you want to acquire the extension (remember to have a user with global administrator permissions for an efficient installation and configuration).
3. Select the environment in which the extension will be installed.
4. Follow the steps given by Business Central to install the Plur-E extension.

Note: Keep in mind that, when installing an extension, Business Central will interrupt the sessions of all users who are using the environment.

5. Once the Plur-E extension is installed, go to the Business Central page called Assisted Setup and select Plur-E Setup to open the Plur-E Wizard and configure it.
6. Follow the terms and conditions in the Plur-E Wizard.
7. The next step will open the Azure Active Directory application of Business Central that will allow you to grant the necessary permissions to Plur-E. Within the window that appears next, click on "Grant Consent".
8. Once the extension is activated, the wizard will allow you to configure the document series that Plur-E can use in the Mobile Application. This list of series will be "Pre-selected" according to the modules purchased on the Plur-E portal.
9. By clicking the "Next" button, you have finished configuring the Plur-E extension.
10. If you search in the Business Central search engine for the Plur-E Setup page, you will see all the settings and the link to the Plur-E web administration portal, where you can configure the modules you have subscribed and configured, for example, the Sales Module.

## Other aspects to consider during installation
### Aspect 1
If you get the following message: "Go to the central business Extensions Manager page and select the Plur-E extension and select the configure option."
1. Once in this section, you must activate the check called "Allow HttpClient Requests".

### Aspect 2
Once the installation of the Plur-E extension is finished, the users and environments must be configured in the Plur-E web portal.
1. In the Environments section of the Plur-E web portal, you can configure the Business Central environments that have the Plur-E extension installed and configured.
2. In the Users section, you can configure the users that will use the mobile application by configuring their subscriptions and available environments.
3. Once the users have been created, they will receive a temporary password to enter the mobile application. Once inside the application, the password can be changed for the convenience of the user who is using it.

## Appendices
### Appendix A
In this appendix, you will find the way to configure a central business user with global administrator permissions.
1. Go to the following link: https://portal.office.com/Adminportal/Home#/users
2. Select the user to which you want to give global permissions.
3. Select the "Manage Roles" option.
4. Check the "Admin Center Access" and then "Global Administrator" options.

It is also recommended to configure the user who is going to install the extension as "Super" in Business Central.