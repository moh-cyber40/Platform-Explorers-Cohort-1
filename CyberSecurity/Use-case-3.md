# Role Based Application Access Package 

## Overview 

This use case outlines the process for a company to create access packages for specific applications based on user teams using Microsoft Entra ID Governance. The goal is to streamline access management by automating the assignment of access packages based on user attributes, ensuring that users have the right access at the right time. 

## Detailed Use Case 

### Scenario: 
A company wants to streamline the process of granting access to specific applications for different user teams. The company has various teams, each requiring access to different sets of applications, groups, and resources. The current manual process is time-consuming and prone to errors. The company aims to automate this process using Microsoft Entra ID Governance to create access packages that bundle the necessary resources for each team. 

### Requirements: 

Automated Access Management: Automate the assignment of access packages based on user attributes such as department, role, and location. 

Enhanced Security: Ensure that users have the appropriate access based on their roles and responsibilities, minimizing the risk of unauthorized access. 

Streamlined Processes: Simplify the process of managing access to multiple resources, making it easier for administrators to handle access requests and reviews. 

Regular Access Reviews: Implement a process to regularly review and remove access when a user's job role changes or they leave the organization. 


### Configuration
- Logged in to the Microsoft Entra ID Governance portal
  <img width="947" alt="role" src="https://github.com/user-attachments/assets/43468d4e-4c54-4716-a605-7ee79e1737bf" />
  
- Navigated to Identity Governance > Entitlement Management.
  <img width="958" alt="role 1" src="https://github.com/user-attachments/assets/50e3486b-6518-40b4-ab50-bcc0ee046207" />

- Clicked on Access Packages > + New access package.
  <img width="955" alt="role 2" src="https://github.com/user-attachments/assets/22ee55bb-a33a-4726-88c0-8192f8c1c418" />
  <img width="949" alt="role 3" src="https://github.com/user-attachments/assets/8dc7d3cc-6cf0-4196-adfa-eb3c5fd96af4" />
  
- Gave a name and description to the access package, and also chose the approriate catalog.
  <img width="607" alt="role 4" src="https://github.com/user-attachments/assets/fcd0060e-77c3-44ac-b589-2d44475dd18a" />

 - Navigated to resource roles to choose appropriate "groups and teams"
   <img width="729" alt="group" src="https://github.com/user-attachments/assets/dcfddeed-013e-4acc-9c16-260a68daabfa" />

 - Navigated to Requests, made sure only users in my directory can request access.
   <img width="670" alt="role 5" src="https://github.com/user-attachments/assets/0c53ad31-ccc1-4b83-af35-97bd5d4a317d" />
   <img width="644" alt="role 6" src="https://github.com/user-attachments/assets/f2d855b2-2d5e-4872-81d7-4d028af8be91" />

 - For the approval, I enabled 2 stages for the approval and approval must be made within 7 days. First approver is the manager approval, Muhammad is assigned for that role.
   <img width="771" alt="stages of approval" src="https://github.com/user-attachments/assets/7b080321-946c-4fa8-a039-98dd844f3862" />

   Second approval is assigned to Chioma
   <img width="646" alt="role 8" src="https://github.com/user-attachments/assets/d5f61aea-a395-411c-b8f5-8815b354b6f8" />

 - Navigated to Requestor information where I set up a question for the requestor which required a short answer.
   <img width="732" alt="role 10" src="https://github.com/user-attachments/assets/0c28e8ad-b4e8-4006-8dd8-2e442fa99a27" />

 - Navigated to Lifecycle where I set the number of days it will take for access to the access package before it expires.
   <img width="744" alt="role 11" src="https://github.com/user-attachments/assets/fa7258cf-0a6c-44d1-aadf-e846b58d1996" />

 - For access reviews. The review frequency is set is to be bi-annually and the number of days is set to be 90 days.
   <img width="661" alt="role 12" src="https://github.com/user-attachments/assets/ac7fd510-6ad2-4cb0-a0d7-87b24015b686" />
   <img width="529" alt="reviewer 1" src="https://github.com/user-attachments/assets/534f5250-1a14-42e2-8403-ec047cee3ae5" />

 - Reviewed the access package and create.
   <img width="775" alt="review + create" src="https://github.com/user-attachments/assets/0afec577-95da-4dc7-ac01-6e2f8073743b" />

## Testing
In testing this configuration, a team member (Denis) was asked to request for  approval so as to test the configuration. He requested for approval and the request went to the first approver (Muhammad) who approved it. After the first stage of approver, the request moved to the second approver (Chioma) who also approved it.
   <img width="418" alt="denis approval request 2" src="https://github.com/user-attachments/assets/ec10aed8-a574-4aec-a918-b9d141e826fb" />

Image below shows the approval history
    <img width="952" alt="approval history" src="https://github.com/user-attachments/assets/dfd39c73-f244-4f14-bb81-3e500c975a9a" />


  








  



