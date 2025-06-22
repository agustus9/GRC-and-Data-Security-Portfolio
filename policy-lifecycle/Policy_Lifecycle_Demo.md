# 📋 Policy Lifecycle Governance Demo

This project demonstrates a simplified lifecycle of a security policy from creation to enforcement and review, aligned with ISO 27001 and NIST guidelines.

---

## 📑 Use Case

An organization needs to enforce a Data Retention Policy that ensures logs are retained for 1 year to meet compliance with ISO 27001:2013 and SOC 2.

---

## 🛠️ Lifecycle Stages

### 1. **Draft**
- Initial draft created by GRC team using Microsoft Word or a policy management tool.
- Reviewed internally for completeness and mapped to ISO control 12.7 (Retention).

### 2. **Review**
- Sent for stakeholder review (Legal, IT, Security).
- Edits incorporated and finalized in the approval workflow.

### 3. **Approval**
- Policy signed off by senior management.
- Document versioned and added to the policy repository.

### 4. **Enforcement**
- Controls implemented via retention rules in logging platforms (e.g., Splunk, Azure Monitor).
- Linked to audit schedules and automated alerts.

### 5. **Review & Update**
- Policy reviewed annually.
- Metrics pulled from logging platforms to validate compliance.

---

## 🔍 Framework Mapping

| Framework | Control Reference | Relevance             |
|-----------|-------------------|------------------------|
| ISO 27001 | A.12.7.1          | Retention of Records   |
| SOC 2     | CC7.2             | Logging/Monitoring     |
| NIST CSF  | PR.IP-1           | Policy Management      |

---

## ✅ Output

This simulation was documented and included as part of my GRC portfolio to demonstrate real-world governance implementation.
