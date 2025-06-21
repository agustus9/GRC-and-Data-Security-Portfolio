# Microsoft Purview DLP Lab

This is a dedicated lab walkthrough for configuring and validating Data Loss Prevention policies using Microsoft Purview.

# Microsoft Purview DLP Lab

This hands-on lab guides you through setting up Data Loss Prevention (DLP) using Microsoft Purview in a simulated enterprise environment.

## 🧪 Lab Objectives
- Understand Microsoft Purview DLP capabilities
- Configure and test data loss policies for sensitive information
- Monitor alerts and simulate incident response

## 🛠️ Lab Sections

1. **Set Up Microsoft Purview (M365 E5 Trial)**  
   - Enable Purview in compliance.microsoft.com  
   - Assign appropriate permissions (`Compliance Data Administrator`)

2. **Define Sensitive Info Types**  
   - Use built-in (e.g., SSNs, Credit Cards) or create custom types

3. **Create DLP Policies**  
   - Choose test workloads (SharePoint, Exchange, OneDrive)
   - Apply policy rules: Detect, block, audit, notify

4. **Simulate Violations**  
   - Upload files with dummy SSNs or payment data  
   - Trigger alert, review policy match, test rule response

5. **Analyze with DLP Reports**  
   - Use Activity Explorer & Alerts dashboard  
   - Refine rules or policy scope

6. **Bonus**: Integrate with Microsoft Defender or Sentinel for escalation

## 📄 Documentation Output
- Screenshots of policies and alerts  
- Summary of test results  
- Recommended improvements

---

🧠 This lab is part of Arthur Mack’s GRC Portfolio. See full portfolio at [https://github.com/agustus9/grc-portfolio](https://github.com/agustus9/grc-portfolio).

