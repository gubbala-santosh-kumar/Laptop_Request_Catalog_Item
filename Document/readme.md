# Laptop Request Catalog – ServiceNow Project

## Project Overview
The Laptop Request Catalog is a ServiceNow-based project designed to streamline and automate the process of requesting laptops within an organization. This system replaces manual request methods such as emails and paper-based forms with a structured and user-friendly digital catalog item in ServiceNow.

The project enables users to request laptops by filling out a standardized form that captures all necessary details such as laptop model, justification, and additional accessories. It improves efficiency, reduces errors, and ensures better request management within the organization.

## Features
- ServiceNow Service Catalog based laptop request system  
- Structured request form with required fields  
- Dynamic form behavior using UI policies  
- Additional accessories option with conditional fields  
- Reset form functionality using UI action  
- Update set creation for easy deployment across instances  
- Export and import functionality using XML update set  
- Tested in multiple ServiceNow instances  

## Technologies Used
- ServiceNow Platform  
- Service Catalog  
- Catalog Variables  
- Catalog UI Policies  
- UI Actions  
- Update Sets  

## Project Modules

### 1. Create Local Update Set
A local update set is created to track all configurations made during the project. All development activities are performed within this update set to ensure easy export and migration.

### 2. Create Service Catalog Item
A catalog item named **Laptop Request** is created under the Hardware category in the Service Catalog. This item allows users to submit laptop requests.

### 3. Add Variables
The following variables are added to the catalog item:
- Laptop Model (Single line text)  
- Justification (Multi-line text)  
- Additional Accessories (Checkbox)  
- Accessories Details (Multi-line text)  

### 4. Catalog UI Policy
A UI policy is implemented to make the **Accessories Details** field visible and mandatory only when the **Additional Accessories** checkbox is selected.

### 5. UI Action
A reset form UI action is created to clear all fields in the form and allow users to refill the request easily.

### 6. Export and Import Update Set
All configurations are captured in an update set and exported as an XML file. This file can be imported into another ServiceNow instance and committed to replicate the project setup.

### 7. Testing
The catalog item is tested to ensure:
- Proper field visibility  
- Mandatory conditions  
- Reset functionality  
- Successful migration between instances  

## Advantages
- Replaces manual request process  
- Structured and user-friendly interface  
- Reduces errors and delays  
- Easy deployment using update sets  
- Efficient request management  

## Limitations
- Depends on ServiceNow platform  
- No advanced approval workflow included  
- Basic implementation for demonstration purposes  

## Future Enhancements
- Automated approval workflow  
- Email notifications  
- Request status tracking  
- Integration with asset management  
- Support for additional hardware requests  

## Conclusion
The Laptop Request Catalog project demonstrates how ServiceNow can be used to automate and manage laptop requests efficiently. It improves accuracy, transparency, and user experience while providing a scalable solution for organizations.
