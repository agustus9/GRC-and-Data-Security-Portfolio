# 🧩 POA&M Workflow (Qualys → ServiceNow Integration)

## Overview

This demo outlines a mock Plan of Action and Milestones (POA&M) workflow showing how vulnerability and compliance findings from Qualys can be automatically transferred into ServiceNow, including tagging, CI reconciliation, and ticket lifecycle handling.

---

## Key Components

- **Qualys**: Source of vulnerability and compliance scan data.
- **MID Server**: Secure channel for integrating Qualys data into ServiceNow CMDB.
- **ServiceNow GRC**: Destination for automated creation of POA&Ms tied to assets and policies.

---

## Lab Flow (Simplified)

1. **Scan Runs in Qualys**
   - VM/PC scan results collected, identifying non-compliance or CVEs.

2. **Tagging & Asset Grouping**
   - Assets tagged (e.g., `PCI-Servers`, `Windows-2016`).
   - Tags drive routing to ServiceNow.

3. **CI Matching (CMDB)**
   - CI reconciliation rules match based on:
     - IP Address
     - Hostname
     - FQDN

4. **POA&M Ticket Created in ServiceNow**
   - Automatically creates:
     - A Security Incident or Change Request
     - Assigns to resolver group
     - Maps to control failure (CIS, NIST, etc.)

5. **Policy Mapping**
   - Maps finding to policy control (e.g., `CIS 1.1.1 - Password Complexity`)
   - Adds compliance reference for audits.

6. **Lifecycle Management**
   - SLA timer starts.
   - Resolver provides remediation notes or requests an exception.
   - Workflow tracks remediation, testing, and closure.

---

## Example Output

- 👨‍💼 Assigned To: Vulnerability Response Team
- 🔐 Finding: Weak password policy on 6 Windows CIs
- 📋 Control: CIS 1.1.1
- 📅 SLA: 14 Days
- 🛠️ Action: Update GPOs, re-test via Qualys, auto-close ticket

---

## Benefits

✅ Faster audit prep  
✅ Traceable remediation  
✅ Stronger policy mapping  
✅ Cross-team accountability

---

## Screenshot Placeholder

(Insert screenshot of POA&M ticket or dashboard here)

---

