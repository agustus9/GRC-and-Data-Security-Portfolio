# 🧪 Qualys Custom Assessment & Remediation – Script Demo

This walkthrough demonstrates how to use Qualys CAR (Custom Assessment and Remediation) to detect and resolve insecure endpoint configurations using scripted logic.

---

## 🔍 Scenario: Enforce Defender Real-Time Protection

**Security Control Goal:**  
Ensure Microsoft Defender’s Real-Time Protection is enabled on all endpoints.

**Standards Mapped To:**  
- **CIS Controls:** 5.1, 5.3  
- **NIST SP 800-53:** SI-3, SI-7  
- **ISO 27001:** A.12.6.1

---

## 🧪 Assessment Script (Groovy)

```groovy
def isDefenderOff = 'powershell -Command "Get-MpPreference | Select -ExpandProperty DisableRealtimeMonitoring"'.execute().text.trim()
if (isDefenderOff == "True") {
    return "Real-time protection is DISABLED"
} else {
    return "Real-time protection is ENABLED"
}

'powershell -Command "Set-MpPreference -DisableRealtimeMonitoring $false"'.execute()
return "Real-time protection has been ENABLED"


---

