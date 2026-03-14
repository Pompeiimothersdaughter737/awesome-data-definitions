# Awesome Data Definitions 🗃️

> A curated collection of standardized data definitions, abbreviations, and naming conventions for enterprise data architecture.

[![Website](https://img.shields.io/badge/Website-mdatool.com-blue)](https://www.mdatool.com)
[![Definitions](https://img.shields.io/badge/Definitions-17,000+-green)](https://www.mdatool.com/definitions)
[![Domains](https://img.shields.io/badge/Domains-6-orange)](https://www.mdatool.com/glossary)

## 📚 What is this?

This repository contains **sample data definitions** from [mdatool.com](https://www.mdatool.com) - the world's largest library of standardized database terminology across 6 industry domains.

Perfect for:
- 🏥 Healthcare data architects
- 💰 Financial data engineers
- 🛒 E-commerce platform builders
- 🚚 Supply chain data modelers
- 💊 Pharmacy system designers
- 💻 Software engineering teams

## 🎯 Industry Coverage

| Domain | Definitions | Sample |
|--------|------------|---------|
| Healthcare | 4,600+ | [View Samples](./healthcare/) |
| Banking & Finance | 2,100+ | [View Samples](./banking-finance/) |
| Retail & E-commerce | 1,600+ | [View Samples](./retail-ecommerce/) |
| Software | 3,300+ | [View Samples](./software/) |
| Pharmacy | 400+ | [View Samples](./pharmacy/) |
| Global Fleet | 400+ | [View Samples](./global-fleet/) |

**Total: 17,000+ verified definitions** | [Browse all →](https://www.mdatool.com)

---

## 📖 Sample Definitions

### Healthcare

**PHI (Protected Health Information)**
```
Definition: Any individually identifiable health information transmitted or maintained 
by a covered entity, protected under HIPAA regulations.

Common Fields:
- patient_id
- medical_record_number
- diagnosis_code (ICD-10)
- procedure_code (CPT)

Standards: HIPAA, HL7 FHIR
```

**HCC (Hierarchical Condition Category)**
```
Definition: Risk adjustment model used by CMS to calculate Medicare Advantage payments 
based on patient health status and predicted healthcare costs.

Common Fields:
- hcc_code
- hcc_description
- risk_score
- capture_date

Standards: CMS-HCC Model V28
```

[**→ See 4,600+ Healthcare definitions**](https://www.mdatool.com/definitions/healthcare)

---

### Banking & Finance

**AML (Anti-Money Laundering)**
```
Definition: Set of procedures and regulations designed to prevent criminals from 
disguising illegally obtained funds as legitimate income.

Common Fields:
- transaction_amount
- suspicious_activity_flag
- kyc_status
- screening_result

Standards: BSA, FinCEN, FATF
```

**SWIFT (Society for Worldwide Interbank Financial Telecommunication)**
```
Definition: Global messaging network for secure financial transactions between banks.

Common Fields:
- swift_code (BIC)
- iban
- wire_reference_number
- settlement_date

Standards: ISO 9362, ISO 20022
```

[**→ See 2,100+ Finance definitions**](https://www.mdatool.com/definitions/banking-finance)

---

## 🛠️ Free Tools

Beyond definitions, [mdatool.com](https://www.mdatool.com) provides free engineering tools:

### [DDL Converter](https://www.mdatool.com/ddl-converter)
Convert DDL between Oracle, PostgreSQL, MySQL, SQL Server, Snowflake
```sql
-- Oracle
CREATE TABLE employees (
    employee_id NUMBER(10),
    hire_date DATE DEFAULT SYSDATE
);

-- Auto-converts to PostgreSQL →
CREATE TABLE employees (
    employee_id INTEGER,
    hire_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### [SQL Linter](https://www.mdatool.com/sql-linter)
Catch security issues and performance problems
```sql
-- Detects:
✗ SELECT * usage
✗ Missing WHERE clause on UPDATE
✗ SQL injection vulnerabilities
✗ Functions on indexed columns
✓ Suggests optimizations
```

### [Naming Auditor](https://www.mdatool.com/naming-auditor)
Enforce consistent naming conventions
```sql
-- Flags inconsistencies:
✗ CustomerID (PascalCase)
✗ product_name (snake_case)
✗ orderDate (camelCase)

✓ Suggests: customer_id, product_name, order_date
```

---

## 📂 Repository Structure
```
awesome-data-definitions/
├── healthcare/
│   ├── common-terms.md
│   ├── hipaa-fields.md
│   └── hl7-fhir-resources.md
├── banking-finance/
│   ├── payment-terms.md
│   ├── regulatory-fields.md
│   └── swift-codes.md
├── retail-ecommerce/
│   ├── product-catalog.md
│   └── order-management.md
├── software/
│   ├── database-terms.md
│   └── api-standards.md
├── pharmacy/
│   └── prescription-fields.md
├── global-fleet/
│   └── logistics-terms.md
└── naming-conventions/
    ├── snake-case-guide.md
    ├── database-standards.md
    └── industry-best-practices.md
```

---

## 🎓 Learn More

- **Blog**: [Engineering guides and best practices](https://www.mdatool.com/blog)
- **Glossary**: [Browse all 17,000+ definitions](https://www.mdatool.com/glossary)
- **Documentation**: [API access and integration](https://www.mdatool.com/docs)

---

## 🤝 Contributing

Want to add definitions or suggest improvements?

1. This is a **sample repository** - full database at [mdatool.com](https://www.mdatool.com)
2. Submit suggestions via [contact form](https://www.mdatool.com/contact)
3. For enterprise contributions, email: admin@mdatool.com

---

## 📜 License

Sample definitions are provided for reference. Full access available at [mdatool.com](https://www.mdatool.com).

---

## ⭐ Support

If you find this helpful:
- Star this repository
- Share with your team
- Follow [@mdatool](https://twitter.com/mdatool) for updates

---

**Built for data professionals, by data professionals.**

[Visit mdatool.com →](https://www.mdatool.com)
