# General Instructions for Mentees

Your goal is to complete your assigned use case while keeping your monthly budget within $50. You can use the Azure Portal or Azure CLI, but ensure you track your resources properly.
## Budgeting and Cost Control

### Set a Budget and Alerts

- Use the Cost Management tool to create a budget with alerts at 50%, 75%, and 90% usage.
- Regularly check cost breakdowns to avoid exceeding the limit.

### Optimize Costs

   -  Use cost-effective resource sizes.
  - Shut down or delete resources when not in use.
    If possible, use auto-scaling or cost-saving features.

## Resource Governance and Monitoring

### Enable Monitoring

  - Set up alerts for CPU, memory, and network usage.
- Log important events for troubleshooting and cost analysis.

### Organize Your Resources

  - Use tags (e.g., Project: XYZ, Owner: YourName) to categorize resources.

### Apply Governance Policies

  - Prevent high-cost configurations.
- Ensure only necessary resources are deployed.

## Security and Access Control

### Protect Your Resources
- Follow security best practices and check for misconfigurations.
-  Regularly review any security recommendations provided by Azure.

### Control Access

   -  Assign minimal permissions needed for the project (least privilege principle).
   -  Do not give unnecessary administrator-level access.

### Secure Remote Access

  - Avoid exposing services directly to the internet unless absolutely necessary.
- Use on-demand access methods instead of leaving access open.

## Implementation Guidelines

### Use Any Allowed Method

  -  You can configure resources through Azure Portal or Azure CLI.
- If using CLI, ensure you understand the commands before running them.

### Document Your Setup

  - Keep a log of what you did (screenshots, CLI commands, design decisions).
  -  Be prepared to explain your architecture and cost decisions.

## Completion Criteria & Evaluation

    ✅ Did you set up a budget and stay within the $50 limit?
    ✅ Did you implement monitoring and governance properly?
    ✅ Did you apply best practices for security and access control?
    ✅ Did you successfully complete your assigned use case?
    ✅ Can you explain your architecture and justify your decisions?
