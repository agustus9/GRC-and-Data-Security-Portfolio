
# 🗂 POA&M Workflow Example – Risk Remediation and Tracking

This document provides an example of a Plan of Action and Milestones (POA&M) workflow used for tracking control deficiencies, mitigation plans, and accountability across teams.

---

## 📌 Use Case

A POA&M is a formal document that identifies security control weaknesses and outlines the steps, resources, and timeline for remediation.

---

## 🛠 Workflow Overview

1. **Control Failure Identified**
   - Example: Windows server failed STIG control for RDP encryption.
   - Trigger: Weekly compliance scan from Qualys Policy Compliance module.

2. **Ticket Created**
   - Assigned in ServiceNow using a POA&M Template.
   - Captures system owner, control ID, and business impact rating.

3. **Risk Analysis**
   - Mapped to NIST 800-53 control (e.g., AC-17).
   - Impact: Medium
   - Likelihood: Moderate
   - Inherent Risk Score: 9

4. **Mitigation Plan Defined**
   - Remediation action: Disable weak ciphers and enforce TLS 1.2
   - Owner: Infrastructure Team
   - Target Remediation Date: 30 days

5. **Milestones Set**
   - Week 1: Submit Change Request
   - Week 2: Apply security settings
   - Week 3: Validate via rescan
   - Week 4: Close POA&M

6. **Status Updates**
   - Documented weekly in POA&M Tracker (Excel or ServiceNow GRC)
   - Status: “In Progress” → “Pending Validation” → “Closed”

7. **Closure Evidence**
   - Screenshots of configuration
   - Updated scan results
   - Change record link

---

## 🔐 Outcome

By following this workflow, the organization ensures traceable, auditable, and accountable risk mitigation aligned with enterprise GRC goals.

