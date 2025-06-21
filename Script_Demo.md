
# ⚙️ Script Demo – Qualys to ServiceNow Integration

This script demo outlines a simplified process for automating Qualys Compliance findings into ServiceNow, enabling real-time POA&M tracking and CI tagging.

---

## 🧩 Script Purpose

- Ingest Qualys policy compliance scan data
- Map findings to Configuration Items (CIs) in ServiceNow
- Automatically generate or update POA&M records
- Add CI Tags based on risk tier or policy failure

---

## 🛠️ Tools and Technologies

- Python (requests, json)
- Qualys API (Compliance Policy & Host List Detection APIs)
- ServiceNow API (CMDB, Security Incident, POA&M modules)
- MID Server / IntegrationHub (for production-grade delivery)

---

## 🧪 Sample Workflow

```python
import requests

# 1. Fetch failed policy hosts from Qualys Compliance API
qualys_base = "https://qualysapi.qualys.com"
auth = ("username", "password")
policy_id = "123456"

response = requests.get(
    f"{qualys_base}/api/2.0/fo/compliance/policy/",
    params={"action": "list", "id": policy_id},
    auth=auth
)

# 2. Parse and normalize data
compliance_data = response.text  # placeholder
# (parse XML or JSON, extract hostnames, controls, status)

# 3. Post findings to ServiceNow
servicenow_instance = "https://devXXXX.service-now.com"
headers = {"Content-Type": "application/json", "Authorization": "Bearer YOUR_TOKEN"}

poam_payload = {
    "short_description": "Qualys Policy Compliance Failure",
    "cmdb_ci": "server123.domain",
    "risk_rating": "Moderate",
    "status": "Open"
}

requests.post(
    f"{servicenow_instance}/api/now/table/u_poam_table",
    headers=headers,
    json=poam_payload
)
```

---

## 📘 Notes

- Ensure secure credentials (e.g., using environment variables or Vault)
- Real-world scripts will include error handling, pagination, retries
- This workflow supports visibility across vulnerability and compliance gaps

---

## ✅ Outcomes

✔️ Automated POA&M creation  
✔️ Faster remediation tracking  
✔️ Risk-aligned CI tagging  
✔️ Improved audit readiness

