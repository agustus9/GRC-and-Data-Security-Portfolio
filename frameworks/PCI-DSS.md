# 📦 PCI-DSS – Payment Card Industry Data Security Standard

## 🔐 Overview

The **Payment Card Industry Data Security Standard (PCI-DSS)** is a globally recognized security standard developed by major credit card companies (Visa, MasterCard, American Express, Discover, and JCB) to ensure that all organizations that process, store, or transmit credit card information maintain a secure environment.

## 🧱 Control Categories (12 Requirements)

| Category                            | Description                                                                 |
|-------------------------------------|-----------------------------------------------------------------------------|
| 1. Install and maintain firewalls   | Protect cardholder data through proper network segmentation                 |
| 2. Secure system passwords          | Avoid vendor-supplied defaults for system passwords                         |
| 3. Protect stored cardholder data   | Use encryption and tokenization to secure sensitive cardholder data         |
| 4. Encrypt transmission             | Secure cardholder data during transmission across public networks           |
| 5. Use antivirus                    | Protect all systems against malware                                         |
| 6. Secure systems and apps          | Develop and maintain secure systems and applications                        |
| 7. Limit access to data             | Restrict cardholder data access to only those who need it                   |
| 8. Unique IDs for access            | Assign a unique ID to each person with computer access                      |
| 9. Physical access control          | Restrict physical access to cardholder data                                 |
| 10. Monitor all access              | Track and monitor all access to network resources and cardholder data       |
| 11. Regular testing                 | Routinely test security systems and processes                               |
| 12. Information security policy     | Maintain a policy that addresses security information for all personnel     |

## 🛠️ Implementation Guidance

- Conduct a **gap analysis** against the current state of your environment.
- Use a **PCI-DSS SAQ (Self-Assessment Questionnaire)** to determine compliance scope.
- Create a **data flow diagram** for cardholder data.
- Enable **centralized logging** for all systems handling sensitive data.
- Integrate with **SIEM tools** to monitor logs and generate alerts.
- Schedule **quarterly ASV scans** and **annual penetration testing**.

## 📎 Helpful Tools & Technologies

- 🔍 Qualys PCI Module
- 🔐 Microsoft Purview DLP for data protection
- 🧾 Splunk for audit logging and alerting
- 🧰 ServiceNow GRC for evidence management
- 📋 Risk Register & POA&M for managing remediation

## 📘 Resources

- [Official PCI-DSS Site](https://www.pcisecuritystandards.org/)
- [Self-Assessment Questionnaires](https://www.pcisecuritystandards.org/document_library)
- [NIST vs PCI-DSS Mapping](https://csrc.nist.gov/publications/detail/white-paper/2019/04/01/pci-dss-vs-nist-standards)

---

