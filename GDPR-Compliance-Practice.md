# GDPR Practice Starter Data

## Data Inventory

| Data Category        | Data Type       | Source             | Storage Location | Purpose of Processing | Data Sensitivity | Data Retention Period | Data Subject Type | Access Rights     | Notes                  |
|----------------------|-----------------|--------------------|------------------|-----------------------|------------------|-----------------------|-------------------|------------------|------------------------|
| Customer Contact Info | Name, Email     | Website Signup     | CRM System       | Marketing             | High             | 2 years               | Customer          | Marketing Team   | Data collected via form |
| Employee Records     | Name, SSN, Email| HR Department      | HR System        | Payroll & HR        | High             | 7 years               | Employee          | HR Department    | Confidential data       |

## Data Flow Mapping

| Data Processed     | Source System       | Destination System   | Data Transfer Method | Frequency  | Security Measures | Responsible Department |
|--------------------|---------------------|----------------------|----------------------|------------|-------------------|------------------------|
| Customer Data      | Website             | CRM System           | HTTPS                | Real-time  | Encryption        | Marketing              |
| Employee Data      | HR System           | Payroll System       | Secure API           | Monthly    | VPN & Encryption  | HR                     |

## Risk & Gap Assessment

| Activity/Process     | GDPR Requirement                     | Current Status | Risk Level | Remediation Actions                         | Responsible Person | Due Date   | Status  |
|----------------------|----------------------------------------|----------------|------------|--------------------------------------------|--------------------|------------|---------|
| Data Storage         | Encrypt all stored personal data     | Partial        | Medium     | Implement full encryption across systems | IT Security Lead   | 2024-06-30 | Pending |
| Data Transfer        | Use secure transfer protocols          | Yes            | Low        | N/A                                        | IT Security Lead   | N/A        | Complete|

## Data Subject Rights Tracker

| Data Subject ID | Request Type    | Date of Request | Status   | Response Date | Notes                     |
|-----------------|----------------|----------------|----------|--------------|---------------------------|
| 12345           | Access         | 2024-05-01     | Pending  |              | Customer requested data  |
| 67890           | Data Erasure   | 2024-05-03     | Completed| 2024-05-05   | Data erased successfully |

---

### How to use:
- Copy everything above.
- Paste into your markdown file (`.md`) on GitHub.
- The tables will display with proper borders and styling.

