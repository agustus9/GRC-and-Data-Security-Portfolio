# Custom Sensitive Information Types – Template & Guide

This guide outlines the key components and template for creating Custom Sensitive Information Types (SITs) in Microsoft Purview.

---

## 🔍 Core Components of a Sensitive Information Type

| Component            | Description                                                                                 |
|----------------------|---------------------------------------------------------------------------------------------|
| Name                 | The display name of your custom SIT                                                         |
| Description          | Optional, used for documentation and internal reference                                     |
| Pattern              | A combination of primary element (Regex or keyword), supporting elements, and validation    |
| Primary Element      | Regex pattern or keyword list used to trigger the match                                     |
| Supporting Elements  | Optional additional keywords or regex patterns to increase confidence                       |
| Confidence Level     | Low, Medium, or High – determines how confident the system is that this is a true match     |
| Proximity            | Defines how close supporting elements must be to the primary element (in characters)        |
| Match Requirements   | Minimum number of elements required for a match to occur (e.g., 1 primary + 1 supporting)   |
| Example Text         | Sample string that matches the defined pattern                                              |

---

## 📌 Sample Template

Use this structure to define your own custom SITs.

| Field               | Example                                                                                       |
|--------------------|-----------------------------------------------------------------------------------------------|
| Name               | Internal Employee ID                                                                          |
| Description        | 6-digit ID prefixed by "INT-" used for internal HR systems                                    |
| Primary Element    | `INT-\d{6}`                                                                                   |
| Supporting Elements| `Employee`, `HR`, `Internal Use Only`                                                         |
| Confidence Level   | High                                                                                           |
| Proximity          | 300 characters                                                                                 |
| Match Requirements | 1 primary + 1 supporting                                                                       |
| Example Text       | "Employee ID: INT-934215. This record is for internal use only by the HR department."         |

---

## 🧠 Tips

- Use [regex101.com](https://regex101.com) to validate your regex before uploading it to Purview.
- Be cautious with short regex patterns — they can create false positives.
- Test custom SITs in a lab using **Test DLP policy mode** before enforcing in production.

---

## 📂 Integration

Place this file in your repo at:  
`grc-portfolio/purview-regex/Custom_Sensitive_Information_Types_Template.md`
