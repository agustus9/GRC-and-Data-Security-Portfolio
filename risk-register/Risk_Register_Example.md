# 📋 Risk Register Example

This is a sample risk register entry designed to showcase GRC portfolio experience using ISO 27001 and NIST-mapped risk scenarios. Each row in the risk register should represent an individual risk scenario affecting a particular system, process, or organizational function.

---

## Example Entry

| **Risk ID** | **Risk Description**                                  | **Asset**             | **Threat**                | **Vulnerability**                        | **Impact** | **Likelihood** | **Risk Score** | **Control**                            | **Owner**        | **Status**      |
|------------|--------------------------------------------------------|------------------------|----------------------------|------------------------------------------|-----------|----------------|----------------|----------------------------------------|------------------|------------------|
| RISK-2025-001 | Outdated OS on key server may lead to exploitation. | Web Server - Prod      | Remote Exploitation       | Unsupported Windows 2012 OS              | High      | Medium         | High           | Upgrade to supported OS & patching     | Infra Manager    | Open             |

---

## Mapping

- **Frameworks Used**:
  - ISO/IEC 27005
  - NIST SP 800-30
  - NIST CSF (Identify → Risk Assessment)
  - CIS Control v8 - Control 04 (Secure Configuration)
  
---

## Sample Risk Response Plan

**Mitigation**: Immediate OS upgrade plan initiated. Temporary firewall rules to restrict unnecessary access.  
**Residual Risk**: Accepted by leadership until full upgrade.  
**POA&M**: Tracked in ServiceNow with 45-day remediation window.

---

## 📎 Related Documents

- `Risk_Register_Template.xlsx` ← spreadsheet template
- `Risk_Register_Example.md` ← this file
- `Policy_Lifecycle_Demo.md` ← linked process for policy tracking

---

## 🧠 Notes

Risk registers are a cornerstone of Governance, Risk, and Compliance (GRC) operations. This file and associated Excel template show your ability to:

- Identify, track, and score risks
- Map controls to frameworks
- Communicate risks across technical and non-technical stakeholders

