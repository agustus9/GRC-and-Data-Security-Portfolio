
# 🔐 Microsoft Purview DLP Simulation Lab – Data Protection in Action

This section documents a simulation lab using Microsoft Purview to implement Data Loss Prevention (DLP) policies across a hybrid environment.

---

## 🎯 Objective

To simulate end-to-end deployment of Microsoft Purview DLP policies for detecting and protecting sensitive data, including PII and financial records, across cloud services and endpoints.

---

## 🧪 Lab Outline

1. **Environment Setup**:
   - Microsoft 365 Compliance Center
   - Purview Permissions (Data Loss Prevention admin role)
   - Demo Exchange Online and OneDrive environment

2. **DLP Policy Design**:
   - Created policies to detect U.S. SSNs, credit card numbers, and custom keywords
   - Defined actions: Audit only, Email notification, and Auto-quarantine

3. **Testing & Validation**:
   - Uploaded test files with simulated sensitive content
   - Triggered policy actions and validated DLP logs via Activity Explorer

4. **DLP Analytics Integration**:
   - Enabled DLP Analytics preview to identify oversharing risks and usage patterns
   - Captured weekly metrics and visualizations

---

## 📁 Files Included

- Policy configurations (JSON snippets)
- Screenshots of DLP hits and analytics dashboard
- Lab simulation notes and outcomes

---

## ✅ Key Outcomes

- Demonstrated Microsoft Purview’s policy effectiveness in a realistic scenario
- Provided audit-ready evidence for GRC evaluations
- Mapped results to ISO 27001:2022 and NIST 800-53 (AC-1, AC-4, SI-4)

---

## 📘 Related Skills

- Microsoft Purview Compliance Center
- DLP Analytics & Activity Explorer
- Regulatory Alignment (ISO, NIST, HIPAA)
