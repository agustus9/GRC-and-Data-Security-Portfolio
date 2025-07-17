# Automation for GRC & Data Security

This section consolidates scripts, tutorials, and resources to automate Governance, Risk, and Compliance (GRC) and Data Security processes using Python and PowerShell. Derived from Cybrary courses, these resources aim to streamline compliance, risk management, vulnerability assessments, and security operations.

## Repository Structure

---

## Sample Content & Examples

### Python for GRC & Data Security
- Automate Vulnerability Scanning: Script to parse output from tools like Nessus or OpenVAS, generating compliance reports.
- Policy Compliance Checks: Script that scans configurations or files to verify adherence to data security policies (e.g., encryption, access controls).


## Sample Content & Examples

### Python for GRC & Data Security
- Automate Vulnerability Scanning: Script to parse output from tools like Nessus or OpenVAS, generating compliance reports.
- Policy Compliance Checks: Script that scans configurations or files to verify adherence to data security policies (e.g., encryption, access controls).

**Example snippet:**
```python
import json

# Example: Parse vulnerability scan report and highlight high-risk issues
with open('scan_report.json') as f:
    report = json.load(f)

high_risks = [issue for issue in report['issues'] if issue['severity'] == 'High']
print(f"High-risk vulnerabilities found: {len(high_risks)}")
for vuln in high_risks:
    print(f"- {vuln['title']} at {vuln['host']}")
---

# List all users with admin privileges
Import-Module ActiveDirectory
Get-ADGroupMember -Identity "Domain Admins" | Select-Object Name, SamAccountName
