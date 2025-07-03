# Controls Mapping Guide for Financial Regulations & Cybersecurity Frameworks

This document provides a comprehensive overview of control identifiers, numbering schemes, and mapping references across major financial regulations and cybersecurity frameworks. It facilitates linking regulatory requirements to standardized controls, assisting compliance and security program development.

---

## 1. Financial Regulations and Their Controls

### A. Sarbanes-Oxley Act (SOX)
- **Control Approach:** Focuses on internal controls over financial reporting.
- **Framework Mapping:** Uses frameworks like **COBIT** (e.g., **DS5**, **ME1**) and **COSO** components.
- **Note:** SOX does not specify control numbers itself; organizations map requirements to these frameworks.

---

### B. PCI DSS (Payment Card Industry Data Security Standard)
- **Main Structure:** 12 Requirements, each with numbered sub-requirements.
- **Examples of Controls:**
  - **1.1:** Establish and maintain firewall configuration standards.
  - **2.2:** Do not use vendor-supplied defaults.
  - **6.4:** Implement security patches.
  - **12.1:** Maintain a security policy.
- **Use:** These numbered requirements serve as controls for compliance audits.

---

### C. GLBA (Gramm-Leach-Bliley Act)
- **Control Approach:** Does not specify control numbers; emphasizes safeguarding customer information.
- **Implementation:** Map to frameworks like **NIST** or **ISO** for controls such as access, encryption, incident response.

---

### D. FISMA (Federal Information Security Management Act)
- **Framework:** Uses **NIST SP 800-53** controls.
- **Key Control Identifiers:**
  - **AC-1:** Access Control Policy & Procedures
  - **IA-2:** Identification & Authentication
  - **SI-4:** System Monitoring
  - **RA-5:** Vulnerability Scanning
- **Note:** Controls are organized into families; each has a specific ID.

---

## 2. Cybersecurity Frameworks and Their Controls

### A. NIST Cybersecurity Framework (CSF)
- **Structure:** Functions, Categories, Subcategories.
- **Control Examples:**
  - **ID.AM-1:** Physical device inventory.
  - **PR.IP-1:** Baseline configurations.
  - **DE.CM-7:** Anomaly detection.
- **Mapping:** Controls are mapped to **NIST SP 800-53** controls.

---

### B. ISO/IEC 27001
- **Control Annex (A.5 – A.18):** 114 controls organized into domains.
- **Examples:**
  - **A.5:** Information Security Policies
  - **A.6:** Organization of Security
  - **A.8:** Asset Management
  - **A.9:** Access Control
  - **A.10:** Cryptography
  - **A.11:** Physical Security
  - **A.12:** Operations Security
  - **A.13:** Communications Security
  - **A.14:** System Acquisition
  - **A.15:** Supplier Security
  - **A.16:** Incident Management
  - **A.17:** Business Continuity
- **Numbering:** Controls identified as **A.x.y** (e.g., **A.9.1.1**).

---

### C. CIS Controls
- **Numbered Controls (1-20):**
  - **1:** Inventory of Devices
  - **2:** Inventory of Software
  - **3:** Vulnerability Management
  - **4:** Admin Privileges
  - **5:** Secure Configuration
  - **6:** Log Monitoring
  - **...** up to Control 20.
- **Use:** Practical, prioritized security controls.

---

## 3. Control Numbering & Mapping Summary Table

| Framework / Regulation | Control Identifiers / Numbers | Description / Notes |
|----------------------------|----------------------------------|---------------------|
| **SOX (via COBIT/COSO)** | COSO Components, COBIT IDs | No specific numbers; mapped via frameworks |
| **PCI DSS** | Requirement 1, 2, 3, ... 12 | Main requirement numbers |
| **GLBA** | Not numbered; mapped to NIST/ISO | Focus on safeguards |
| **FISMA / NIST 800-53** | AC-1, IA-2, SI-4, RA-5, etc. | Family controls with IDs |
| **NIST CSF** | ID.AM-1, PR.IP-1, DE.CM-7 | Subcategory IDs |
| **ISO 27001** | A.5, A.6, A.8, A.9, etc. | Annex A controls |
| **CIS Controls** | 1, 2, 3, ..., 20 | Practical controls |

---

## 4. Linking Controls in Your GitHub Repository

Use this reference to:
- Map standards to internal policies
- Link control IDs with compliance artifacts
- Automate assessments and reporting
- Demonstrate traceability

---

## 5. Links to Standards & Resources

- [NIST SP 800-53 Controls](https://pages.nist.gov/800-53-revision-5-controls/)
- [ISO/IEC 27001 Controls Annex A](https://www.iso.org/standard/54534.html)
- [CIS Controls Version 8](https://www.cisecurity.org/controls/cis-controls-list/)
- [PCI DSS v4.0 Requirements](https://www.pcisecuritystandards.org/pci_security/)

---

## How to Add This to Your GitHub Repository

### Step-by-step instructions:

1. **Copy the entire markdown content above.**

2. **Create a new file in your local repo or on GitHub:**
   - If using GitHub web interface:
     - Navigate to your repository.
     - Click **Add file** > **Create new file**.
     - Name the file: `Controls_Mapping_Guide.md`.

3. **Paste the copied markdown content** into the editor.

4. **Commit the new file:**
   - Enter a commit message, e.g., "Add controls mapping guide."
   - Click **Commit new file**.

5. **(Optional) Clone your repo locally**:
   - Use `git clone` to clone your repo.
   - Save the markdown file on your machine.
   - Use `git add Controls_Mapping_Guide.md`, then `git commit -m "Add controls mapping guide"` and `git push` to upload.

---

If you'd like, I can also prepare this as a downloadable file and provide the raw markdown content for copying. Just let me know!
