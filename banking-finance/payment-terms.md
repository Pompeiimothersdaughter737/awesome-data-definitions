# Banking & Finance: Payment Terms

## Account Information

### account_number
**Type:** VARCHAR(20)  
**Description:** Unique bank account identifier  
**Standards:** ISO 13616 (IBAN format for international)  
**Example:** 1234567890

### routing_number
**Type:** VARCHAR(9)  
**Description:** ABA routing transit number (US banks)  
**Standards:** ABA RTN  
**Example:** 021000021

### swift_code
**Type:** VARCHAR(11)  
**Description:** Bank Identifier Code for international transfers  
**Standards:** ISO 9362  
**Example:** CHASUS33XXX

---

## Transaction Data

### transaction_amount
**Type:** DECIMAL(18,2)  
**Description:** Monetary amount of transaction  
**Important:** ALWAYS use DECIMAL, never FLOAT for money  
**Example:** 1234.56

### transaction_type
**Type:** VARCHAR(50)  
**Description:** Category of transaction  
**Values:** DEPOSIT, WITHDRAWAL, TRANSFER, FEE, INTEREST  
**Standards:** ISO 20022

### transaction_date
**Type:** TIMESTAMP  
**Description:** When the transaction occurred  
**Timezone:** Store in UTC  
**Example:** 2024-03-14 15:30:00

---

## Compliance & Security

### kyc_status
**Type:** VARCHAR(20)  
**Description:** Know Your Customer verification status  
**Values:** PENDING, VERIFIED, REJECTED, EXPIRED  
**Standards:** FATF, AML regulations

### aml_screening_result
**Type:** VARCHAR(20)  
**Description:** Anti-Money Laundering screening outcome  
**Values:** CLEAR, FLAGGED, BLOCKED  
**Standards:** FinCEN, BSA

### risk_score
**Type:** DECIMAL(5,2)  
**Description:** Transaction risk assessment (0-100)  
**Example:** 12.50

---

## International Payments

### iban
**Type:** VARCHAR(34)  
**Description:** International Bank Account Number  
**Format:** 2 letter country code + 2 check digits + up to 30 alphanumeric  
**Example:** GB82WEST12345698765432  
**Standards:** ISO 13616

### bic
**Type:** VARCHAR(11)  
**Description:** Bank Identifier Code (same as SWIFT code)  
**Standards:** ISO 9362  
**Example:** DEUTDEFF

---

[View all 2,100+ Finance definitions →](https://www.mdatool.com/definitions/banking-finance)
