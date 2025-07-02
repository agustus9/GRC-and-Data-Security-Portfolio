# 📊 Financial Regulations and Cybersecurity Frameworks

This section summarizes key U.S. and global financial regulations and frameworks critical to data security, compliance, and risk management. Each file in this folder explores one regulation or framework in more depth.

## 📂 Available Frameworks and Regulations

| Regulation/Framework | Description |
|----------------------|-------------|
| [📦 GLBA](financial-regulations/GLBA.md) | Gramm-Leach-Bliley Act – Focused on protecting consumer financial privacy. |
| [📦 SOX](financial-regulations/SOX.md) | Sarbanes-Oxley Act – Financial reporting and IT General Controls. |
| [📦 FFIEC](financial-regulations/FFIEC.md) | Federal Financial Institutions Examination Council – Includes CAT and URSIT. |
| [📦 PCI DSS](financial-regulations/PCI_DSS.md) | Payment Card Industry Data Security Standard – Cardholder data protection. |
| [📦 NYDFS 500](financial-regulations/NYDFS_500.md) | NY Department of Financial Services – Cybersecurity rules for financial firms. |
| [📦 GDPR](financial-regulations/GDPR.md) | General Data Protection Regulation – EU-wide data privacy rules. |
| [📦 ISO 27001](financial-regulations/ISO_27001.md) | International standard for Information Security Management Systems. |
| [📦 NIST 800-53](financial-regulations/NIST_800_53.md) | Baseline security and privacy controls for federal systems and beyond. |
| [📦 CPRA / CCPA](financial-regulations/CPRA_CCPA.md) | California data privacy laws – U.S. equivalent to GDPR. |
| [📦 Basel III](financial-regulations/Basel_III.md) | International regulation covering liquidity, risk, and capital for banks. |
| [📦 DORA](financial-regulations/DORA.md) | EU Digital Operational Resilience Act – IT risk management in financial services. |
| [📦 FATF](financial-regulations/FATF.md) | Anti-money laundering standards and financial transaction monitoring. |
| [📦 SWIFT CSCF](financial-regulations/SWIFT_CSCF.md) | Secure financial messaging practices. |
| [📦 OCC Guidelines](financial-regulations/OCC_Guidelines.md) | Risk management practices from the U.S. banking regulator. |
| [📦 HITRUST CSF](financial-regulations/HITRUST_CSF.md) | Control framework aligning HIPAA, NIST, PCI-DSS, and ISO 27001. |

---

📁 Each link above opens a detailed `.md` file on the regulation or framework.

---

# 📦 GLBA – Gramm-Leach-Bliley Act

**Focus**: Protection of consumer financial information

**Key Components**:
- **Financial Privacy Rule** – Requires financial institutions to provide privacy notices.
- **Safeguards Rule** – Mandates a written information security plan.
- **Pretexting Rule** – Prevents social engineering to gain access to personal data.

**Applies To**: Financial institutions and service providers

**Control Areas**:
- Risk assessments
- Encryption & data protection
- Third-party due diligence

---

# 📦 SOX – Sarbanes-Oxley Act

**Focus**: Internal controls over financial reporting

**Key Sections**:
- **Section 302**: Corporate responsibility for financial reports
- **Section 404**: Management assessment of internal controls
- **Section 802**: Retention and destruction of financial records

**IT Controls**:
- IT General Controls (ITGC)
- Access management
- Audit trail integrity

---

# 📦 FFIEC – Federal Financial Institutions Examination Council

**Focus**: Uniform standards for U.S. financial institution cybersecurity

**Key Tools**:
- **Cybersecurity Assessment Tool (CAT)**: Risk and maturity assessment
- **Uniform Rating System for IT (URSIT)**

**Assessment Areas**:
- Cyber risk management
- Third-party risk
- Incident response
- Governance

---

# 📦 PCI DSS – Payment Card Industry Data Security Standard

**Focus**: Secure handling of cardholder data

**Applies To**: Any organization that stores, processes, or transmits credit/debit card data

**Key Requirements**:
1. Install firewalls
2. Encrypt transmission
3. Restrict access to cardholder data
4. Regularly test security systems

**Compliance**: Validated via Self-Assessment Questionnaires (SAQs) or formal audits

---

# 📦 NYDFS 23 NYCRR 500

**Focus**: Cybersecurity for New York-based financial services firms

**Mandates**:
- Appoint a CISO
- Conduct annual risk assessments
- Implement encryption and access controls
- Report cybersecurity events within 72 hours

**Applies To**: Banks, insurers, and financial institutions regulated in NY

---

# 📦 GDPR – General Data Protection Regulation (EU)

**Focus**: Privacy and protection of EU citizen data

**Core Rights**:
- Right to access
- Right to erasure (Right to be forgotten)
- Data portability
- Consent management

**Organizational Requirements**:
- Appoint a Data Protection Officer (DPO)
- Perform Data Protection Impact Assessments (DPIA)
- Maintain data processing records

---

# 📦 ISO/IEC 27001

**Focus**: Information Security Management System (ISMS)

**Framework Elements**:
- Risk-based approach
- Controls aligned with Annex A
- Continuous improvement via PDCA (Plan-Do-Check-Act)

**Common Artifacts**:
- Asset inventories
- Security policies
- Access control matrices

---

# 📦 NIST SP 800-53

**Focus**: Security and privacy controls for federal information systems

**Control Families**:
- AC: Access Control
- AU: Audit and Accountability
- CM: Configuration Management
- IR: Incident Response
- RA: Risk Assessment
- SC: System and Communications Protection

**Versions**: Rev 5 (current), Rev 4 (legacy)

---

# 📦 CPRA / CCPA – California Privacy Laws

**Focus**: Consumer rights and business obligations

**Consumer Rights**:
- Know what data is collected
- Request deletion
- Opt-out of sale
- Non-discrimination for exercising privacy rights

**Business Requirements**:
- Data classification
- Notice at collection
- Vendor contracts and risk assessments

---

# 📦 Basel III

**Focus**: Bank liquidity, capital adequacy, and operational risk

**Cybersecurity Relevance**:
- Operational risk from IT disruptions
- ISMS for financial continuity
- Controls for confidentiality, integrity, and availability

**Implemented By**: Global systemically important banks (G-SIBs)

---

# 📦 DORA – Digital Operational Resilience Act (EU)

**Focus**: ICT risk management in EU financial institutions

**Requires**:
- Incident reporting
- Digital resilience testing
- ICT third-party risk management
- Governance and accountability

**Effective**: 2025

---

# 📦 FATF – Financial Action Task Force

**Focus**: Anti-money laundering (AML) and countering terrorism financing

**Key Components**:
- Customer due diligence
- Suspicious activity monitoring
- Risk-based approach
- Compliance controls for crypto transactions

**Evaluates**: Member countries’ frameworks

---

# 📦 SWIFT Customer Security Controls Framework (CSCF)

**Focus**: Secure financial messaging between institutions

**Controls**:
- Secure zone architecture
- Multi-factor authentication
- Audit trail logging
- Endpoint hardening

**Mandatory for**: All SWIFT users

---

# 📦 OCC Guidelines

**Issued By**: U.S. Office of the Comptroller of the Currency

**Focus**: Risk management for banks and financial services

**Principles**:
- Third-party risk
- Cloud governance
- Board-level accountability
- Due diligence and monitoring

**Applies To**: National banks and federal savings associations

---

# 📦 HITRUST CSF

**Focus**: Unified control framework for healthcare and financial industries

**Integrates**:
- HIPAA
- NIST SP 800-53
- ISO 27001
- PCI-DSS

**Used For**:
- Compliance assessments
- Data protection programs
- Risk management automation
