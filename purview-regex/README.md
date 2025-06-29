# 📘 Purview Regex Overview & Custom Sensitive Information Types

This section contains key regex patterns and methods used to define **Custom Sensitive Information Types (SITs)** in **Microsoft Purview**.

## 🔍 What Are Custom Sensitive Information Types?

Microsoft Purview allows organizations to define custom sensitive data detection rules based on:

- **Regular expressions (Regex)**
- **Confidence levels**
- **Supporting evidence (e.g., keywords)**
- **Occurrences and proximity**
- **Custom validation logic**

These rules are useful for identifying organization-specific data types like employee IDs, medical record numbers, or internal codes.

---

## 📁 Included Files

- [`Regex_Custom_Sensitive_Information_Types.md`](./Regex_Custom_Sensitive_Information_Types.md):  
  Contains example regex patterns for detecting sensitive info like US Social Security Numbers, custom Employee IDs, financial routing numbers, and more.

---

## ✅ Example Use Cases

| Sensitive Type | Regex Example | Notes |
|----------------|----------------|-------|
| SSN (US) | `\b\d{3}-\d{2}-\d{4}\b` | Matches 123-45-6789 |
| Employee ID | `EMP\d{6}` | Matches EMP123456 |
| Internal Case Code | `CASE-[A-Z]{4}-\d{3}` | Matches CASE-ABCD-001 |
| Financial Routing | `\b\d{9}\b` | 9-digit US bank routing |

---

## 📎 How to Use in Purview

When creating a **Custom Sensitive Information Type** in the Microsoft Purview compliance portal:

1. Go to **Data Classification > Sensitive Info Types**
2. Click **Create**, and choose **Custom**
3. Define:
   - Regex match pattern
   - Supporting keywords (optional)
   - Confidence levels
   - Proximity rules
4. Save and publish

---

## 📌 Related Links

- [Microsoft Docs – Custom Sensitive Info Types](https://learn.microsoft.com/en-us/microsoft-365/compliance/sit-create-custom?view=o365-worldwide)
- [Regex Cheatsheet (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Cheatsheet)

---

**Arthur Mack**  
- **GitHub GRC Portfolio**: [https://github.com/agustus9/grc-portfolio](https://github.com/agustus9/grc-portfolio)
- **LinkedIn**: [https://www.linkedin.com/in/arthur-m-24a2a81ba/](https://www.linkedin.com/in/arthur-m-24a2a81ba/)
