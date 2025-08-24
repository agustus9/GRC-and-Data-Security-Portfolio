# Microsoft Purview – DLP Simulation Lab

![Microsoft Purview Lab Banner](Microsoft_Purview_Lab_Banner.png)

This GitHub-based lab simulates how Microsoft Purview’s DLP tools can be structured and implemented using prewritten templates and keyword dictionaries.

> 🧪 This is a simulated training lab, not a production environment.

---

| Focus Area          | Key Features & Tools                                                                                                 |
|---------------------|---------------------------------------------------------------------------------------------------------------------|
| **Data Security**   | - Data Loss Prevention (DLP)                                                                                      |
|                     | - Information Barriers                                                                                            |
|                     | - Information Protection                                                                                          |
|                     | - Insider Risk Management                                                                                         |
|                     | - Privileged Access Management                                                                                    |
| **Risk & Compliance** | - Audit                                                                                                         |
|                     | - eDiscovery                                                                                                      |
|                     | - Compliance Manager                                                                                              |
|                     | - Data Lifecycle Management                                                                                       |
|                     | - Communication Compliance                                                                                        |
| **Data Governance** | - Data Catalog                                                                                                    |
|                     | - Data Estate Insights                                                                                            |
|                     | - Data Map                                                                                                        |
|                     | - Data Policy                                                                                                     |
|                     | - Data Sharing                                                                                                    |

---

## 🧬 1. Sensitive Information Types

Microsoft Purview offers built-in and custom **Sensitive Information Types (SITs)** for identifying data like credit cards, SSNs, or healthcare info.

You can also create **Custom SITs** using:
- **Regex patterns**
- **Keyword dictionaries**
- **Supporting evidence (confidence levels)**

📸 Screenshot:  
![Purview Policy View](Purview_Screenshot_1.png)

---

## 🛡️ 2. DLP & Policy Simulation

Use our Excel-based **DLP policy template** to simulate rule creation for Microsoft Purview.

📄 Download: [DLP_Policy_Template_SAMPLE.xlsx](DLP_Policy_Template_SAMPLE.xlsx)

Policy Components:
- Conditions (e.g., detects “financial terms”)
- Actions (e.g., block download, alert admin)
- Scopes (e.g., SharePoint, Teams, Exchange)

📸 Screenshot:  
![Purview Policy View](Purview_Screenshot_2.png)

---

## 🗂️ 3. Keyword Dictionaries

Purview supports uploading custom keyword lists to create **dictionary-based SITs**.

📄 Sample Files:
- [financial_terms.txt](../purview-keywords/financial_terms.txt)
- [healthcare_terms.txt](../purview-keywords/healthcare_terms.txt)

🧭 Import Instructions:  
[Keyword Dictionary Setup Guide](../purview-keywords/README.md)

---

> 🔄 This lab continues to evolve with additional templates, rules, and dashboards.  
