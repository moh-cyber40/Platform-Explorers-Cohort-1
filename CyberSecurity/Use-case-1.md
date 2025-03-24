# Mitigating Fraudulent Emails at Contoso

## Company Overview: 
Contoso is a mid-sized organization with 300 users located in the United States and Western Europe. The company has been experiencing a significant challenge with fraudulent emails being delivered to end users' mailboxes, posing a risk of phishing attacks and potential data breaches. 

## Problem Statement:  
Contoso's email system is currently vulnerable to fraudulent emails, which are being delivered to end users' mailboxes. This issue has raised concerns about the security of sensitive information and the potential for phishing attacks. The company needs to implement a robust solution to mitigate this risk and protect its users, especially VIP users such as the CEO, CFO, and CISO. 

## Objective:  
To seek advice from a security analyst on the resolution of the fraudulent email issue, including the type of Microsoft 365 plan that can be purchased, features that can help mitigate the concern, and configuration steps that can be taken to protect the organization. The analyst needs to configure their recommended policies to solve the business problem. Additionally, the analyst should take screenshots of the configuration steps and upload them to their GitHub repository, explaining their thought process and any potential implications of the new policies. The analyst should also determine if these steps should be applied to a group of test users first before being rolled out to the entire organization, ensuring the protection of VIP users. 
Also, the analyst should advise on how to get stakeholder reports of mail flow to and from the organization. 

## Recommended Microsoft 365 Plan:
I recommend Micorsoft Defender for Office Plan 2 because it offers comprehensive protection against advanced threats, including phishing, malware, and business email compromise. It also includes advanced threat hunting, automation, cross-domain XDR capabilities.

## Features to Mitigate Fraudulent Emails:
1. Safe Attachments: Scans all email attachments for malware and other malicious content.
2. Safe Links: Protects users by checking URLs in emails and Office documents in real-time.
3. Anti-Phishing Policies: Uses machine learning models to detect and block phishing attempts.
4. Threat Explorer: Provides visibility into threats and allows for proactive threat hunting.
5. Attack Simulation Training: Helps train users to recognize and avoid phishing attempts.

## Configuration of Policies:
1. Enable Safe Attachments
   - Go to Microsoft 365 defender portal (security.microsoft.com)
     <img width="953" alt="m365 defender portal" src="https://github.com/user-attachments/assets/37122558-b847-4c1e-b1fc-f8c205bfce2a" />
   - Click the dropdown arrow under "Email and Collaboration "Navigate to Policies & rules > Threat policies > Safe Attachments
     <img width="956" alt="policies and rules" src="https://github.com/user-attachments/assets/613a606b-a83d-46f2-ac40-daf387bfacbc" />
     <img width="959" alt="threat policies" src="https://github.com/user-attachments/assets/75fb2c31-65e5-4bce-9942-ce44aa00ffaa" />
     <img width="959" alt="safe attachment" src="https://github.com/user-attachments/assets/1e091ee3-f743-47cc-9e4a-d5e6dd5b1d22" />
   - Create a new policy and configure it to scan all messages and attachments
     Give the policy a name which is compulsory and also a description which is optional
     <img width="954" alt="new policy" src="https://github.com/user-attachments/assets/cd86db88-1f9f-4cee-87b1-c7b11cc7134a" />
  
     here, I added required user
     <img width="959" alt="policy setting" src="https://github.com/user-attachments/assets/6ac90e87-77b6-40d2-8e77-8429bc361c85" />
   - Here I reviewed and submitted the policy
     <img width="956" alt="review policy" src="https://github.com/user-attachments/assets/3dd25e4f-2bc4-4f3c-8cff-3916e69b4360" />
     <img width="946" alt="attachment policy done" src="https://github.com/user-attachments/assets/f773577d-128b-4907-bdb7-bf26c7a731e1" />
     Policy (safe attachment policy) have been added successfully which is seen in the screenshot below.
     <img width="947" alt="safe attachement done" src="https://github.com/user-attachments/assets/a501b421-d8d5-4bbb-944b-8d71a2612d60" />

2. Enable Safe Links:
   - In the Microsoft 365 Defender portal, I navigated to Policies & rules > Threat policies > Safe Links
     <img width="959" alt="safe links" src="https://github.com/user-attachments/assets/78a42c3a-118a-4c4e-8073-0b4ad7944e39" />
   - I created a new policy, enabled URL scanning, and applied it to required users
     <img width="959" alt="safe links 2" src="https://github.com/user-attachments/assets/20125b47-393a-4d5b-866e-e3b942580a9d" />
     <img width="959" alt="safe links 3" src="https://github.com/user-attachments/assets/8cb06c69-532b-47f0-a846-78e156fad38a" />
     <img width="959" alt="safe links 4" src="https://github.com/user-attachments/assets/0ec160ba-b011-4e35-9b59-eec00341a86f" />
  
     here, I chose how I want users to be notified. I went with default notification text
     <img width="953" alt="safe links 5" src="https://github.com/user-attachments/assets/993e541a-09e7-403c-afca-dcdca963be58" />
   - I reviewed the policy before submitting.
     <img width="959" alt="safe link 6" src="https://github.com/user-attachments/assets/9bc3037f-5620-498d-a345-56335b0047af" />
     <img width="959" alt="safe link 7" src="https://github.com/user-attachments/assets/0708b835-78d8-4bf9-84a3-f4cc4ab460a8" />

3. Configuration of anti-phishing policy:
   - Navigate to Policies & rules > Threat policies > Anti-phishing
     <img width="959" alt="anti phishing" src="https://github.com/user-attachments/assets/50c9ca08-c3e7-465a-bd00-6e8e6efcf504" />
    - I Created a new policy, which enables impersonation protection, and applied it to all users
      <img width="949" alt="anti phishing 2" src="https://github.com/user-attachments/assets/f0b9d509-f960-4d5f-bc72-91c1eb582db3" />
      <img width="956" alt="anti phishing 3" src="https://github.com/user-attachments/assets/e1f5f992-d7cb-48a1-bed1-47ea8733145c" />
      <img width="953" alt="anti phishing 4" src="https://github.com/user-attachments/assets/205c92d3-dfb1-48a5-bfff-58474b435579" />
      <img width="959" alt="anti phishing 5" src="https://github.com/user-attachments/assets/e6e33d69-2249-40ac-9d28-ff5b3477950f" />
      <img width="959" alt="anti phishing 6" src="https://github.com/user-attachments/assets/c49cf860-f557-4fd1-909e-d1703df00c43" />
      <img width="959" alt="anti phishing 7" src="https://github.com/user-attachments/assets/5a911295-ca96-44b8-b3fc-c95f62724cc1" />
      <img width="959" alt="anti phishing 8" src="https://github.com/user-attachments/assets/f6015495-f906-44e5-bd53-0bccae951d2e" />
     - Here, I reviewed the policy before submitting
       <img width="959" alt="anti phishing 9" src="https://github.com/user-attachments/assets/81d1c1d4-8b66-4c53-aa95-e912358c8756" />
       <img width="955" alt="anti phishing 10" src="https://github.com/user-attachments/assets/a70507b4-65c8-4588-86ab-db30515e2bfe" />

4. Implementation of Attack Simulation Training:
   - On your security page, go to Attack Simulation Training
     <img width="955" alt="simulation" src="https://github.com/user-attachments/assets/fd6d65bb-7612-4a37-884a-2edf5e5cbd04" />
    - click the simulation tab and "launch a simulation"
      <img width="959" alt="simulation 2" src="https://github.com/user-attachments/assets/5e622f04-494a-4fa8-bd73-3110bb564b47" />
    - I Selected a technique and clicked next, then I entered a name for the simulation
      <img width="959" alt="simulation 3" src="https://github.com/user-attachments/assets/bb47fc50-0b1a-4416-98f1-f7a632f4874b" />
     - Select a payload and login page
       <img width="956" alt="simulation 4" src="https://github.com/user-attachments/assets/64261063-6816-4797-b6ec-cb603e5ec5b4" />
      - Select targeted user(s)
        <img width="959" alt="simulation 5" src="https://github.com/user-attachments/assets/f2086923-e445-48b3-ad6b-b89ec3dd0a2a" />
       - Select end user notification
        <img width="959" alt="simulation 6" src="https://github.com/user-attachments/assets/474fb922-eabf-4e59-8e68-7311e81b55b7" />
       - Reviewed simulation, submit and launch.
        <img width="959" alt="simulation 7" src="https://github.com/user-attachments/assets/6f7ebfc0-f4f4-4149-9134-f2129c71e737" />
       - Here, Simulation is in progress
        <img width="959" alt="simulation 8" src="https://github.com/user-attachments/assets/a692837d-5309-4be4-831b-9c50c01f73a0" />

## Potential Implications:
   1. Positive Implications
      - Enhanced Security: The new policies significantly reduce the risk of phishing attacks and data breaches
      - User Awareness: Attack Simulation Training improves user awareness and reduces the likelihood of successful phishing attempts
   2. Challenges and Considerations
      - User Experience: Some users might find the additional security measures (e.g. attachment scanning) slightly intrusive. Clear communication about the importance of these measures can help mitigate any resistance
      - False Positives: There might be instances of legitimate emails being flagged as suspicious. Regular monitoring and fine-tuning of policies can help minimize false positives

By carefully considering these factors, Contoso can effectively enhance its email security and protect its users from fraudulent emails and phishing attacks.

## Testing and Rollout Strategy:
   - Test Group: Apply these policies to a small group of users first so as to ensure that the configurations work as expected without disrupting business operations
   - Full Rollout: After successful testing, the policies should be rolled out to the entire organization to ensure comprehensive protection

 ## Stakeholder Reports
 To generate mail flow reports for stakeholders:
    1. Access the Exchange Admin Center (EAC):
       - Go to Microsoft 365 admin center and click "Reports" 
       <img width="959" alt="reports" src="https://github.com/user-attachments/assets/46b76824-0283-498a-a971-c1bc731f7c88" />
       - Click "exchange mail flow reports" it will take you to "Exchange Admin Center" at admin.exchange.microsoft.com
       <img width="958" alt="reports 2" src="https://github.com/user-attachments/assets/a12b65d0-00c9-4ba3-b451-a7962ba8bf55" />
       - Click on "mail flow" under "reports"
       <img width="959" alt="reports 3" src="https://github.com/user-attachments/assets/1125bade-a602-4d4b-9dcb-0320e7f66bd7" />
       - Select the desired report (e.g., inbound messages, outbound messages)
       <img width="959" alt="reports 4" src="https://github.com/user-attachments/assets/c1832147-f7f2-4b25-b24a-c11b9fac845c" />
       - Customize the report parameters and generate the report
       <img width="959" alt="reports 5" src="https://github.com/user-attachments/assets/89fa7087-cd1b-4b37-8455-b25cf9641bd8" />
       - Click on "Export" to generate[download report in excel format and share with stakeholders.





       

 
 
 
 
 









 














    

     
