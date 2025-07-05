# Lab 2: Configure Auto-Labeling Policies for Specific Data Types (PII, PCI)

## Objective
Create and deploy auto-labeling policies that automatically detect and classify sensitive data such as PII (Personally Identifiable Information) and PCI (Payment Card Industry) data across organization’s Microsoft 365 environment.

---

## Prerequisites
- Administrative access to Microsoft Purview & Compliance portal
- Existing sensitivity labels (e.g., "PII", "PCI") or create new labels
- Sample data containing sensitive information for testing

---

## Steps

### 1. Sign in to Microsoft Purview & Microsoft 365 Compliance Center
- Visit [https://compliance.microsoft.com](https://compliance.microsoft.com)
- Sign in with appropriate admin credentials

### 2. Create or Confirm Sensitivity Labels
- Navigate: Data classification > Sensitivity labels
- Create new labels if needed:
  - **Name:** PII / PCI
  - **Description:** Labels for sensitive data types
  - Configure label settings (encryption, access restrictions, etc.)

### 3. Create Auto-Labeling Policy
- Navigate: Data classification > Auto-labeling policies
- Click **"+ Create policy"**

### 4. Configure Policy Settings
- **Name:** `Auto-Label PII & PCI Data`
- **Description:** Automates classification of PII and PCI data

### 5. Select Data Locations
- SharePoint sites
- OneDrive accounts
- Exchange mailboxes
- Teams chats & channels

### 6. Define Sensitive Data Types
- Select built-in classifiers:
  - US Social Security Number (SSN)
  - Credit Card Number
- Set detection thresholds (e.g., detect if at least 1 match)

### 7. Assign Labels
- Choose the sensitivity labels (e.g., "PII", "PCI") to apply automatically

### 8. Set Actions & Notifications
- Auto-apply labels
- Notify users (optional)
- Restrict override permissions

### 9. Review & Create
- Review all settings
- Enable test mode if desired
- Click **Create**

---

## 10. Validation & Testing
- Upload sample documents containing fake PII / PCI data
- Verify labels are automatically applied
- Check detection logs and reports

---

## Additional Tips
- Fine-tune detection thresholds based on false positives
- Expand detection to other sensitive data types
- Automate reporting via Power BI or Sentinel

---

## Sample PowerShell for Policy Listing (Optional)
```powershell
# Connect to Microsoft Graph
Connect-MgGraph -Scopes "InformationProtectionPolicy.Read.All"

# List existing auto-labeling policies
Get-MgInformationProtectionPolicy
