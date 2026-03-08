 Automating Employee Data 

" Project Description"
This project demonstrates how employee data can be automatically imported into the ServiceNow platform using **Import Sets** and **Transform Maps**. The system allows bulk employee records to be uploaded through an Excel dataset and automatically transformed into the **User table** in ServiceNow.

The project also demonstrates the concept of **Dot Walking**, which allows accessing related information from another table without opening that record directly. By using dot walking, related fields such as department, email, and manager information can be automatically retrieved when a user is assigned to an incident.

Additionally, the project shows how **Dictionary Override** can be used to customize field behavior in extended tables by setting a default priority value in the Incident table.

This automation helps reduce manual data entry, improves efficiency, and ensures accurate relationship mapping between ServiceNow tables.


"Workflow"
Excel File  
↓  
Import Set Table  
↓  
Transform Map  
↓  
User Table  
↓  
Relationship Mapping using Dot Walking  
↓  
Priority Default Configuration using Dictionary Override

" Project Milestones"

Milestone 1 – Automating Employee Data Import
- Create employee dataset using Excel.
- Upload the dataset using **Import Sets → Load Data**.
- ServiceNow creates an **Import Set table** to temporarily store data.
- Create a **Transform Map** to move data from Import Set table to the **User table (sys_user)**.
- Use **Mapping Assist** to map fields like department, manager, and email.
- Execute the transform process to insert employee records into the User table.

 Milestone 2 – Relationship Mapping using Dot Walking
- Open the **Incident form**.
- Configure the form layout using **Configure → Form Layout**.
- Add fields:
  - assigned_to.department
  - assigned_to.email
  - assigned_to.manager
- When a user is selected in the **Assigned To** field, the related information such as department and email is automatically retrieved using **Dot Walking**.

 Milestone 3 – Priority Default using Dictionary Override
- Open the **Incident table**.
- Locate the **Priority field** in the dictionary.
- Create a **Dictionary Override** for the Incident table.
- Set the **default priority value** for incident records.
- This allows customizing the priority field behavior specifically for the Incident table.



 Technologies Used
- ServiceNow Developer Instance
- Import Sets
- Transform Maps
- Dot Walking
- Dictionary Override
- Excel Dataset



 "Demo Video"
(Add your Google Drive demo link here)

https://drive.google.com/file/d/14ETCiDbpG1VhtOjBKe9LcrtREBNjpobW/view?usp=sharing

"Team Project"
Naan Mudhalvan Project

Team ID : SWTID-2026-1009
Team Size : 4
Team Leader : SALMA BEGAM S
Team member : SALIMUNNISA Z
Team member : RIFAYA SULTHANA B
Team member : SAVITHA K S  

