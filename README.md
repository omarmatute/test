# Youse Add-on
## An example of how to extend the SAP functional.

This add-on contains additional functions to help SAP not do.

The SDK business objects (DI API) connect to the database directly using the ODBC-protocol. They do not communicate with any of the SAP Business One client components

## Components
  
1. It generates a consecutive when foreign suppliers are created.
2. New route in the menu with access to the balance sheet report.
3. The payment assistant includes two functionalities:

    3.1 Exclusion of accounts for payment wizard process.
    
    3.2 Complete accounting entries after executing the wizard updating the fields (Policy, Invoice number, Product, Branch, Branch office, Endorsement, Claim number, Updated by wizard = Y).

##  Architecture
The add-on connects only once after logging in to SAP through DI-API.

### Dependences

 ![Libs](/libs.PNG "Libs")
 
## Setup

The add-on is a Windows Application and is developed in .NET c# and add the COM libraries `SAPbouiCOM` and `SAPbobsCOM` of the SAP DI-API.

The installation of the add-on can be done from the server or by work station in each of the SAP users.
