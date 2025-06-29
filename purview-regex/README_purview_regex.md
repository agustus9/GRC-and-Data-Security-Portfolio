# Microsoft Purview – Regex Expressions & Custom Sensitive Information Types

This folder contains sample regular expressions (regex) and configuration examples for building **Custom Sensitive Information Types** (SITs) in Microsoft Purview.

## 📁 Folder Structure

```
purview-regex/
├── README_purview_regex.md      # Overview and guidance (this file)
├── Regex_Custom_Sensitive_Information_Types.md
├── patterns/
│   └── [Regex patterns categorized by data type]
└── labs/
    └── [Lab exercises for regex-based detection and configuration]
```

---

## 🔍 What Are Custom Sensitive Information Types?

Custom SITs allow organizations to define their own criteria for detecting sensitive information using:

- **Regex patterns**
- **Keyword lists**
- **Confidence levels**
- **Supporting evidence (e.g., proximity, match count)**

## 🧠 Key Use Cases

- Detect proprietary IDs, tokens, internal codes
- Identify company-specific financial or health data
- Implement detection aligned with industry-specific regulations

## 🛠️ Sample Topics

- U.S. driver’s license patterns by state
- Employee ID and internal tracking formats
- Financial patterns (e.g., routing numbers, account formats)
- Custom PII combinations

---

## ✅ Next Steps

- Review and test regex samples inside `/patterns/`
- Explore guided exercises inside `/labs/`
- Integrate validated regex into Microsoft Purview custom SIT creation

---

## 🧩 Helpful Resources

- [Microsoft Docs: Custom Sensitive Information Types](https://learn.microsoft.com/en-us/microsoft-365/compliance/custom-learn-dlp-sit)
- [Regex101.com](https://regex101.com/) for building and testing expressions
- [Microsoft Purview Documentation](https://learn.microsoft.com/en-us/microsoft-purview/)

