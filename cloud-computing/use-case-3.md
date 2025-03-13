# Use Case 3: Hybrid Cloud Resource Management 
## Background:
Contoso, with 50 employees, needs to extend its hybrid cloud capabilities. The company wants to manage resources across both their Azure environment and on-premises (which is represented by Azure VMs in this case). They want a solution to manage their Azure VMs from a single location, with governance, security, and monitoring integrated into their workflow. 
## Use Case Objective:
Provide a solution that enables Contoso to manage their Azure VMs as if they were on-premises servers using Azure Arc, even though Azure VMs are not traditionally managed by Azure Arc.
## Design and Architecture:
- Hybrid Management: The solution should allow Contoso to manage their Azure VMs using Azure Arc by recognizing them as on-prem servers.
- Security and Monitoring: Set up monitoring to track the health, security, and compliance of these VMs.
- Cost Efficiency: The architecture should take advantage of cost-efficient VM configurations while staying within the budget.
- Resource Governance: Implement governance controls to ensure compliance with corporate policies.
## Implementation:
- Step 1: Create an Azure VM. This will represent Contoso’s on-prem resource.
- Step 2: Use PowerShell commands to connect this Azure VM to Azure Arc, making it appear as an on-prem server.
- Step 3: Configure monitoring and governance to track the health and compliance of the Azure VM.
