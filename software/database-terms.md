# Software: Database Terms

## Primary Keys

### id
**Type:** BIGINT AUTO_INCREMENT  
**Description:** Surrogate primary key  
**Best Practice:** Always use BIGINT, never INT (future-proof)  
**Example:** 1, 2, 3...

### uuid
**Type:** UUID / CHAR(36)  
**Description:** Universally unique identifier  
**Format:** 8-4-4-4-12 hexadecimal  
**Example:** 550e8400-e29b-41d4-a716-446655440000

---

## Timestamps

### created_at
**Type:** TIMESTAMP DEFAULT CURRENT_TIMESTAMP  
**Description:** Record creation timestamp  
**Timezone:** Store in UTC, convert in application layer

### updated_at
**Type:** TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP  
**Description:** Last modification timestamp

---

[View all 3,300+ Software definitions →](https://www.mdatool.com/definitions/software)
