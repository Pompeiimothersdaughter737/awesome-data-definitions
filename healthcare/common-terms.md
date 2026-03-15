# Healthcare Common Terms

## Patient Demographics

### patient_id
**Type:** BIGINT  
**Description:** Unique identifier for a patient across the healthcare system  
**Standards:** HL7 FHIR Patient.id  
**Example:** 123456789

### medical_record_number (MRN)
**Type:** VARCHAR(50)  
**Description:** Hospital-specific patient identifier  
**Standards:** HL7 v2 PID-3  
**Example:** MRN-2024-001234

### date_of_birth
**Type:** DATE  
**Description:** Patient's birth date (YYYY-MM-DD)  
**Standards:** HIPAA, HL7 FHIR  
**Privacy:** PHI - Protected Health Information

---

## Clinical Data

### diagnosis_code
**Type:** VARCHAR(10)  
**Description:** ICD-10 diagnosis code  
**Standards:** ICD-10-CM  
**Example:** E11.9 (Type 2 diabetes mellitus)

### procedure_code
**Type:** VARCHAR(10)  
**Description:** CPT procedure code  
**Standards:** CPT (Current Procedural Terminology)  
**Example:** 99213 (Office visit)

---

[View all 4,600+ Healthcare definitions →](https://www.mdatool.com/definitions/healthcare)
