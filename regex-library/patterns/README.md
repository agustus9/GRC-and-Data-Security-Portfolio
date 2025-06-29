# 📚 Regex Pattern Library

This directory contains a curated set of regular expressions designed to detect various types of sensitive data.

## 🧾 Contents

| Pattern Name          | Description                         | Usage                          |
|-----------------------|-------------------------------------|--------------------------------|
| `email_address.md`    | Matches email addresses             | Used in data loss policies     |
| `us_ssn.md`           | U.S. Social Security Number         | PII detection                  |
| `credit_card.md`      | Credit card formats (Visa, etc.)    | PCI DSS and payment security   |
| `custom_id.md`        | Internal employee ID format         | Internal tracking/classifiers  |

## ✅ Best Practices

- Always test regex patterns using sample data.
- Document edge cases and limitations.
- Align each pattern with Microsoft Purview classification needs.
- Consider combining regex with keyword evidence and proximity indicators.
