# 🔍 Regex Expressions for Microsoft Purview Sensitive Information Types (SITs)

This section includes custom regex patterns to detect sensitive information types within Microsoft Purview DLP policies.

## 📌 Common Custom Regex Patterns

### 1. Employee ID (Format: EMP-123456)
```
EMP-\d{6}
```

### 2. Internal Invoice Number (Format: INV/2023/00123)
```
INV\/\d{4}\/\d{5}
```

### 3. Financial Account Number (Format: ACCT-1234-5678-9012)
```
ACCT-\d{4}-\d{4}-\d{4}
```

### 4. Project Code (Format: PRJ-SECURITY-2024)
```
PRJ-[A-Z]+-\d{4}
```

### 5. U.S. Routing Number (9 Digits)
```
\b\d{9}\b
```

### 6. Client ID (Format: CL-XXXX-YYYY)
```
CL-\d{4}-\d{4}
```

---

## 💡 Tips for Regex in Microsoft Purview

- Regex is **case-sensitive by default**
- Use `(?i)` prefix to enable case-insensitive matching
- Combine with supporting **keywords** for higher confidence
- Validate using **test policies and labels** before enforcing in production

## ✅ Example Use Case

To detect `CL-1234-5678` with supporting keywords like `"Client ID"`, `"Customer Identifier"` within 50 characters:

- **Regex**: `CL-\d{4}-\d{4}`
- **Supporting Keywords**: `["Client ID", "Customer Identifier"]`

