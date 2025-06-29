
# 🔐 Custom Sensitive Information Types in Microsoft Purview

Microsoft Purview allows the creation of custom Sensitive Information Types (SITs) to identify and protect proprietary or organization-specific data patterns not covered by built-in types.

These custom SITs often use Regular Expressions (Regex), keyword dictionaries, or both to match unique data formats.

---

## 📘 Examples of Custom Sensitive Information Types

### 1. Internal Employee ID
- **Format:** EMP-XXXXX
- **Regex:** `EMP-\d{5}`
- **Example Matches:** `EMP-43829`, `EMP-00001`

---

### 2. Incident Ticket ID
- **Format:** INC#######
- **Regex:** `INC\d{7}`
- **Example Matches:** `INC1234567`

---

### 3. Custom Classification Labels
- **Regex:** `CONFIDENTIAL\s*-\s*[A-Z0-9 ]+`
- **Example Matches:** `CONFIDENTIAL - PROJECT HYPERION`, `CONFIDENTIAL - CLIENT ALPHA`

---

### 4. Proprietary Project Codes
- **Format:** PRJ-YYYY-NNN
- **Regex:** `PRJ-\d{4}-\d{3}`
- **Example Matches:** `PRJ-2025-001`, `PRJ-2023-452`

---

### 5. Custom Financial Account Number
- **Format:** 8 digits followed by 2-letter department code
- **Regex:** `\d{8}-[A-Z]{2}`
- **Example Matches:** `12345678-AR`, `87654321-FN`

---

## 📎 How to Use in Microsoft Purview

1. Go to **Data Classification > Sensitive Information Types**
2. Click **+ Create** to add a new custom SIT
3. Choose **Regex pattern detection**
4. Paste your regex
5. (Optional) Add keywords to increase accuracy
6. Test your SIT with sample data
7. Deploy it in **DLP Policies** or **Information Protection labels**

For more details, visit the [Microsoft Docs](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitive-information-type-learn-about?view=o365-worldwide)

---

## 🧠 Best Practices

- Use **confidence levels** and **supporting evidence (keywords)** to reduce false positives
- Test patterns in **test tenants** or limited-scope policies
- Document each regex with use case and contact owner in your organization
