# Pharmacy: Prescription & Medication Fields

## Prescription Information

### prescription_id
**Type:** BIGINT  
**Description:** Unique prescription identifier  
**Standards:** NCPDP  
**Example:** 1234567890

### ndc_code
**Type:** VARCHAR(11)  
**Description:** National Drug Code - FDA standard drug identifier  
**Format:** 5-4-2 (labeler-product-package)  
**Example:** 00378-1805-10  
**Standards:** FDA NDC Directory

### rxnorm_code
**Type:** VARCHAR(20)  
**Description:** RxNorm Concept Unique Identifier  
**Standards:** NIH RxNorm  
**Example:** 197361

---

## Medication Details

### drug_name
**Type:** VARCHAR(255)  
**Description:** Medication generic or brand name  
**Example:** Lisinopril 10mg Tablet

### dosage_form
**Type:** VARCHAR(50)  
**Description:** Physical form of medication  
**Values:** TABLET, CAPSULE, LIQUID, INJECTION, CREAM, PATCH  
**Standards:** FDA Dosage Forms

### strength
**Type:** VARCHAR(50)  
**Description:** Drug strength with unit  
**Format:** [Amount] [Unit]  
**Example:** 10 mg, 500 mg/5 mL

### quantity_dispensed
**Type:** DECIMAL(10,2)  
**Description:** Amount of medication given to patient  
**Example:** 30.00 (for 30 tablets)

---

## Compliance & Safety

### dea_schedule
**Type:** VARCHAR(5)  
**Description:** DEA controlled substance schedule  
**Values:** C-I, C-II, C-III, C-IV, C-V, NULL (non-controlled)  
**Standards:** DEA Controlled Substances Act

### refills_remaining
**Type:** INT  
**Description:** Number of refills left on prescription  
**Range:** 0-11 (controlled substances limited)

### prescriber_npi
**Type:** VARCHAR(10)  
**Description:** National Provider Identifier of prescribing physician  
**Standards:** CMS NPI  
**Example:** 1234567890

---

[View all 400+ Pharmacy definitions →](https://www.mdatool.com/definitions/pharmacy)

