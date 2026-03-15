# Retail & E-commerce: Order Management

## Order Information

### order_id
**Type:** BIGINT  
**Description:** Unique order identifier  
**Example:** 1001234567

### order_number
**Type:** VARCHAR(50)  
**Description:** Human-readable order reference  
**Format:** ORD-YYYY-NNNNNN  
**Example:** ORD-2024-001234

### order_status
**Type:** VARCHAR(50)  
**Description:** Current order state  
**Values:** 
- PENDING
- CONFIRMED
- PROCESSING
- SHIPPED
- DELIVERED
- CANCELLED
- REFUNDED

---

## Product Data

### product_sku
**Type:** VARCHAR(100)  
**Description:** Stock Keeping Unit - unique product identifier  
**Example:** SHIRT-BLU-M-001

### unit_price
**Type:** DECIMAL(10,2)  
**Description:** Price per unit (NEVER use FLOAT for money!)  
**Example:** 29.99

---

[View all 1,600+ Retail definitions →](https://www.mdatool.com/definitions/retail-ecommerce)

