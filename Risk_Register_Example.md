
# 📋 Risk Register Example – Governance, Risk & Compliance Portfolio

This file demonstrates a sample risk register format used in Governance, Risk, and Compliance (GRC) programs to track, assess, and manage organizational risk.

---

## 📌 Objective

To provide a working example of a risk register for identifying, scoring, prioritizing, and tracking IT and cybersecurity risks across an enterprise.

---

## 🧱 Structure Overview

Each row in the risk register typically includes:

- **Risk ID** – Unique identifier
- **Risk Description** – Summary of the threat or issue
- **Likelihood (1–5)** – Probability of occurrence
- **Impact (1–5)** – Severity if realized
- **Risk Score** – Product of likelihood and impact
- **Control Mapping** – Linked to ISO 27001, NIST, CIS, etc.
- **Mitigation Strategy** – Actions to reduce risk
- **Risk Owner** – Person/Team responsible
- **Status** – Open, In Progress, Accepted, Mitigated

---

## 🧾 Example Entry

| Risk ID | Risk Description                              | Likelihood | Impact | Score | Control Mapping     | Mitigation Plan                       | Owner       | Status      |
|---------|------------------------------------------------|------------|--------|-------|----------------------|----------------------------------------|-------------|-------------|
| RSK-001 | Unauthorized access to AWS S3 buckets         | 4          | 5      | 20    | ISO 27001 A.9, NIST AC-6 | Implement IAM policies, enable logging | Cloud Team  | In Progress |
| RSK-002 | Unpatched Windows servers                     | 5          | 4      | 20    | CIS CSC 3, NIST SI-2   | Integrate WSUS with automated patching | Infra Team  | Open        |
| RSK-003 | Data loss from misconfigured OneDrive sharing | 3          | 5      | 15    | ISO 27001 A.8, NIST SI-12 | Apply Purview DLP, limit share scope   | Security Ops | Mitigated   |

---

## ✅ Key Benefits

- Aligns with GRC reporting needs for internal/external audit
- Enables visibility across technology and business units
- Supports regulatory readiness (HIPAA, SOC 2, PCI-DSS, etc.)

---

## 📘 Related Skills

- Risk Assessment & Prioritization
- ISO 27001/NIST/CIS Mapping
- Policy Governance
- Excel/Google Sheets Register Management
