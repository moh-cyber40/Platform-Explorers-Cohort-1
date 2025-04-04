# Device Management and Zero Trust Strategy 

## Overview 

Contoso, an organization with 500 users located in South Africa and East Europe, has recently purchased Microsoft 365 E5 licenses. They aim to manage their Windows and iOS company-assigned devices, protect these devices using Microsoft Defender for Endpoint, and implement a Zero Trust strategy with Multi-Factor Authentication (MFA) to ensure only compliant endpoints can access Microsoft 365 applications. 

## Device Configuration and Compliance Policies 

To manage user devices effectively, Contoso wishes to implement the following device configuration and compliance policies using Microsoft Intune: 

### Device Compliance Policies: 

#### Windows Devices: 

Require BitLocker encryption. 

Ensure Secure Boot is enabled. 

Require code integrity. 

Specify minimum and maximum OS versions 

Minimum: Windows 10 22H2 (Build 19045.5608) 

Maximum: Windows 11 24H2 (Build 26100.3476) 

#### iOS Devices: 

Enforce device passcode. 

Require encryption. 

Specify minimum and maximum OS versions. 

Minimum: iOS 16.1.1 

Maximum: iOS 18.1.1 


### Device Configuration Policies: 

Windows Devices: 

Configure Windows Update settings. 

Set up Windows Defender Antivirus. 

iOS Devices: 

Configure email profiles. 

## Microsoft Defender for Endpoint Implementations 

To protect Windows and iOS devices, Contoso can configure the following implementations using Microsoft Defender for Endpoint: 

### Windows Devices: 

Enable real-time protection. 

Configure network protection. 

Set up attack surface reduction rules. 

Enable endpoint detection and response (EDR). 

Configure automated investigation and response (AIR) capabilities. 

### iOS Devices: 

Enable web protection to guard against phishing and unsafe network connections. 

Configure network protection. 

Set up jailbreak detection. 

Integrate with Intune for device compliance and conditional access policies. 

## Sample Policies and Screenshots 

To provide a comprehensive guide, include sample policies and screenshots of the configuration steps. This will help Contoso's IT team understand the implementation process and ensure a smooth rollout. 

## Report of Research and Findings 

Prepare a detailed report summarizing the research and findings, including the benefits of the proposed policies, potential challenges, and recommendations for successful implementation. This report should serve as a reference for Contoso's IT team and stakeholders. 


## Configuration of Device Compliance Policies

## Steps in configuring windows devices
- Logged in to Microsoft Intune admin center at (intune.microsoft.com) as shown below
  <img width="959" alt="windows" src="https://github.com/user-attachments/assets/195414a9-7d19-4d90-8780-da4faef3d292" />
- Navigated to "Devices"
  <img width="957" alt="windows 1" src="https://github.com/user-attachments/assets/2a44581e-9027-46dd-b031-423f1817b4c7" />
  Under "compliance" I selected "policies" and clicked on "create policy"
  <img width="957" alt="windows 2" src="https://github.com/user-attachments/assets/535ca568-8c1f-4130-bba8-6221835d840e" />
  Under platform, I selected "windows 10 and later" and hit the create button
  <img width="950" alt="windows 3" src="https://github.com/user-attachments/assets/9ea2bfbf-a589-440d-9190-890a22ddb645" />
  I gave the policy a name as shown below
  <img width="956" alt="windows 4" src="https://github.com/user-attachments/assets/967e3f29-6723-4b46-a0fe-cd5e50aeb497" />
  Under compliance, I configured the policy to require bitlocker, secure boot, and code integrity. I also set the minimum OS version as windows 10 and maximum as windows 11 as shown below
  <img width="959" alt="windows 5" src="https://github.com/user-attachments/assets/b54a7730-91f6-4c4c-9059-8950c9b1579d" />
  I added all devices to be compliant to this policy
  <img width="958" alt="windows 6" src="https://github.com/user-attachments/assets/7c7925ff-e9a4-401c-ac33-143ccb657e65" />
  I reviewed and created the policy
  <img width="956" alt="windows 7" src="https://github.com/user-attachments/assets/ece089ea-ee25-4c32-a908-78b413f82e33" />

## Steps in configuring iOS devices
- Under Devices go to compliance and create policy. I selected iOS/iPadOS under "platform"
  <img width="959" alt="ios" src="https://github.com/user-attachments/assets/7cab9429-dcc1-45ff-8de3-0c7beb4854a3" />
  I gave my policy a name as shown below
  <img width="958" alt="ios 2" src="https://github.com/user-attachments/assets/6bb490dd-9beb-4adc-be17-4d1ccefc3047" />
  I enabled passcode
  <img width="959" alt="ios 3" src="https://github.com/user-attachments/assets/8d513f38-2658-4b5c-bb30-bcc4d53c08ab" />
  I added all devices to the group (Included group)
  <img width="959" alt="ios 4" src="https://github.com/user-attachments/assets/ac65ac8e-870a-4ec0-8e45-0fee4c2e8b93" />
  The policy was reviewed and created.
  <img width="959" alt="ios5" src="https://github.com/user-attachments/assets/62c46221-ce3a-4146-9fb6-b2cf0b90a117" />

## Configuration of Microsft Defender for Endpoint

# Windows Devices
  - After logging to Microsoft Intune Admin Center, navigate to "Endpoint Security" and click antivirus
    <img width="959" alt="endpoint" src="https://github.com/user-attachments/assets/776c9359-8131-4887-8371-224faa96b0be" />
  - Select Create Policy and choose the appropriate platform and profile as shown below. Click "create"
    <img width="956" alt="endpoint 1" src="https://github.com/user-attachments/assets/d6a77faa-2f76-453a-9589-572a1f883860" />
  - Gave the policy a name and move to configuration settings.
    <img width="953" alt="endpoint 2" src="https://github.com/user-attachments/assets/46db9723-c22f-4a0a-80b6-feac1842043d" />
    <img width="955" alt="endpoint 3" src="https://github.com/user-attachments/assets/11b122b7-8096-41bc-b8ca-c2f668c5cd17" />
    <img width="959" alt="endpoint 4" src="https://github.com/user-attachments/assets/8fe51f01-dccf-4e72-ac56-48fddede226f" />
    <img width="950" alt="endpoint 5" src="https://github.com/user-attachments/assets/7d6709fc-8a88-48cf-b8fb-655c148a2ef4" />
    <img width="959" alt="endpoint 6" src="https://github.com/user-attachments/assets/39a9f521-c76d-49de-9c97-8450095a98c1" />
    <img width="958" alt="endpoint 7" src="https://github.com/user-attachments/assets/39a0fe9d-ed3e-4adb-afd6-b2e788622fc1" />
  - Reviewed the created policy and save.
    <img width="959" alt="endpoint 8" src="https://github.com/user-attachments/assets/5df7786d-0db8-4185-86b0-7ff08c127d8b" />

## Steps in Setting up attack surface reduction rules

- On Microsoft Intune Admin Center, navigate to endpoint security and select "Attack Sueface Reduction" and create policy.
  <img width="955" alt="endpoint 9" src="https://github.com/user-attachments/assets/357b1618-ebd2-43c1-a067-c3f81451ec67" />
- Select the appropriate platform and profile. Then select create.
  <img width="957" alt="endpoint 10" src="https://github.com/user-attachments/assets/adc976ee-016e-451c-a1ca-44b3223d91c4" />
- Gave the policy a name
  <img width="956" alt="endpoint 11" src="https://github.com/user-attachments/assets/25d9f87a-1c50-4fdd-93f7-86e7d8389da0" />
- Review the policy and save.
  <img width="952" alt="endpoint 12" src="https://github.com/user-attachments/assets/1189cd28-4b5b-4082-92b5-53792b8ee96e" />

## Steps in Configuring endpoint detection and response (EDR) policy
 - On Microsoft Intune Admin Center, navigate to endpoint security and select "Endpoint detection and response" and create new policy.
   <img width="959" alt="endpoint 13" src="https://github.com/user-attachments/assets/2be2a3a3-13ed-4765-b35e-614a3690f50f" />
 - Select the appropriate platform and profile. Then select create
   <img width="954" alt="endpoint 14" src="https://github.com/user-attachments/assets/e3a4edc6-6e99-411d-adb7-1db2ec4ce2af" />
 - Gave the policy a name
   <img width="959" alt="endpoint 15" src="https://github.com/user-attachments/assets/2f000f7e-0203-4377-af39-83db606e4790" />
   

   






















  




 
