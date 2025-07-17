# Automation for GRC & Data Security

This section consolidates scripts, tutorials, and resources to automate Governance, Risk, and Compliance (GRC) and Data Security processes using Python and PowerShell. These resources aim to streamline compliance, risk management, vulnerability assessments, and security operations.

---

### Python for GRC & Data Security
- Automate Vulnerability Scanning: Script to parse output from tools like Nessus or OpenVAS, generating compliance reports.
- Policy Compliance Checks: Script that scans configurations or files to verify adherence to data security policies (e.g., encryption, access controls).

### Python for GRC & Data Security
- Automate Vulnerability Scanning: Script to parse output from tools like Nessus or OpenVAS, generating compliance reports.
- Policy Compliance Checks: Script that scans configurations or files to verify adherence to data security policies (e.g., encryption, access controls).

# Python script
echo "# Example vulnerability scan parser" > Automation-GRC-DataSecurity/Python-for-Cybersecurity/Example1-AutomatedVulnerabilityScanning.py

# PowerShell script
echo "# Example: List AD users with admin privileges" > Automation-GRC-DataSecurity/PowerShell-for-Security-Professionals/Example1-AutomatedUserAccessAudit.ps1

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
# Import Active Directory module
Import-Module ActiveDirectory

# Define the group(s) that represent admin privileges
$adminGroups = @("Domain Admins", "Enterprise Admins", "Schema Admins")

# Initialize an array to hold results
$adminUsers = @()

# Loop through each admin group and get its members
foreach ($group in $adminGroups) {
    Write-Output "Members of $group:"
    try {
        $members = Get-ADGroupMember -Identity $group -Recursive | Where-Object { $_.ObjectClass -eq 'user' }
        foreach ($member in $members) {
            # Get user details
            $user = Get-ADUser -Identity $member.SamAccountName -Properties Name, SamAccountName, Enabled
            $status = if ($user.Enabled) { "Enabled" } else { "Disabled" }
            $adminUsers += [PSCustomObject]@{
                Group      = $group
                Name       = $user.Name
                Username   = $user.SamAccountName
                Status     = $status
            }
        }
    } catch {
        Write-Warning "Could not retrieve members of $group. Are you running with sufficient permissions?"
    }
}

# Output the list of admin users
$adminUsers | Format-Table -AutoSize

