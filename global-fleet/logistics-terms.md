# Global Fleet: Logistics & Transportation

## Shipment Tracking

### tracking_number
**Type:** VARCHAR(100)  
**Description:** Unique shipment identifier  
**Format:** Carrier-specific (varies)  
**Example:** 1Z999AA10123456784 (UPS)

### bol_number
**Type:** VARCHAR(50)  
**Description:** Bill of Lading number - legal shipping document  
**Example:** BOL-2024-001234

### container_number
**Type:** VARCHAR(11)  
**Description:** ISO 6346 shipping container identifier  
**Format:** 4 letters + 7 digits  
**Example:** ABCU1234567

---

## Vehicle Information

### vin
**Type:** VARCHAR(17)  
**Description:** Vehicle Identification Number  
**Standards:** ISO 3779  
**Example:** 1HGBH41JXMN109186

### license_plate
**Type:** VARCHAR(20)  
**Description:** Vehicle registration plate number  
**Example:** ABC-1234

### odometer_reading
**Type:** INT  
**Description:** Total distance traveled (in miles or km)  
**Example:** 45678

---

## Route & Location

### origin_address
**Type:** VARCHAR(500)  
**Description:** Starting location of shipment  

### destination_address
**Type:** VARCHAR(500)  
**Description:** Final delivery location  

### estimated_arrival
**Type:** TIMESTAMP  
**Description:** ETA for shipment delivery  

### actual_arrival
**Type:** TIMESTAMP  
**Description:** Actual delivery timestamp  

---

[View all 400+ Fleet definitions →](https://www.mdatool.com/definitions/global-fleet)

