# **Lab 1: Using Data Classification and Sensitivity Labels in Microsoft Purview**

---

## 🎯 **Objective**

Learn how to **create**, **apply**, and **manage** **sensitivity labels** and **data classifications** to **protect organizational data** within **Microsoft Purview** and **Microsoft 365** environments.

---

## 📝 **Prerequisites**

- Access to **Microsoft Purview** & **Microsoft 365 Compliance Center**  
- Permissions: **Compliance Administrator**, **Information Protection Administrator**, or equivalent  
- Basic understanding of **data sensitivity** and **classification concepts**

---

## 📂 **Starter Files**

| **File Name** | **Description** |
| -------------- | --------------- |
| `sensitivity-labels.json` | Sample JSON configuration for labels |
| `Sample_Confidential_Document.docx` | Sample document labeled confidential |
| `Sample_Public_Report.pdf` | Sample report for public data |
| *Screenshot placeholders* | For documenting the process |

---

## 🚀 **Step-by-Step Instructions**

---

### **1. Sign in to Microsoft Compliance Center**

- Navigate to: **[https://compliance.microsoft.com](https://compliance.microsoft.com)**  
- Sign in with your **administrator account**

---

### **2. Create Sensitivity Labels**

**🔹 Option A: Use the GUI**

- Navigate to **Data classification > Sensitivity labels**  
- Click **"+ Create a sensitivity label"**  
- **Fill in label details:**
  - **Name**: e.g., **Confidential**  
  - **Description**: e.g., *Highly sensitive data requiring encryption and restricted access*  
  - **Color**: Choose a color for label visualization

- **Configure label settings:**
  - **Encryption**: Enable and define permissions
  - **Content Marking**: Add headers, footers, or watermarks
  - **Access Restrictions**: Define who can access or use this label

- Click **Save** to create the label

---

### **3. Publish Sensitivity Labels**

- After creating labels, go to **Label Policies**  
- Click **"+ Publish labels"**  
- **Select labels** to publish  
- **Specify users/groups** who will see/apply the labels  
- Configure additional settings as needed  
- Finish and **publish**

---

### **4. Apply Labels to Content**

**🔹 In Word, Excel, PowerPoint:**

- Open your document  
- In the **Sensitivity** button in the toolbar, select the label (e.g., Confidential)  
- The label applies visual markings and security settings automatically

**🔹 In SharePoint/OneDrive:**

- Use the **Label** column or label policies to classify files

---

### **5. Verify and Manage Labels**

- Use the **Microsoft Purview** portal to **review labeled data**  
- Adjust label policies or permissions as needed  
- Monitor **label usage** and **compliance reports**

---

## 💡 **Additional Tips**

- **Use auto-labeling policies** based on content patterns or sensitive info types  
- **Review and update labels regularly** to reflect organizational changes  
- **Educate users** on applying labels correctly for maximum security

---

## 🖼️ **Visual Aids & Placeholders**

*Insert screenshots here:*

- Navigating to Sensitivity Labels  
- Creating a label  
- Publishing labels  
- Applying labels in documents

---

## 📝 **Summary**

- **Sensitivity labels** help classify and **protect data** based on **sensitivity**  
- Labels can be applied **manually** or **automatically**  
- Proper management ensures **compliance** and **data security**

---

