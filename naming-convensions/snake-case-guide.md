# Snake Case Naming Guide

## Why Snake Case?

Snake case (`snake_case`) is the most readable and widely adopted standard for database naming:

✅ **Readable:** `customer_first_name` vs `customerFirstName`  
✅ **Case-insensitive:** Works in all SQL dialects  
✅ **No quoting needed:** Unlike `"CustomerFirstName"`  
✅ **Industry standard:** Used by PostgreSQL, Snowflake, Redshift

---

## Table Naming

### ✅ DO:
```sql
customers
orders
order_items
customer_addresses
product_categories
```

### ❌ DON'T:
```sql
tbl_customers          -- No prefixes
Customers              -- No PascalCase
customer               -- Use plural
cust                   -- No abbreviations
```

---

## Column Naming

### ✅ DO:
```sql
customer_id            -- Singular for IDs
first_name
last_name
email_address
created_at
updated_at
is_active              -- Boolean prefix: is_, has_, can_
total_amount
order_count
```

### ❌ DON'T:
```sql
CustomerID             -- No PascalCase
firstName              -- No camelCase
fName                  -- No abbreviations
email                  -- Be specific: email_address
createdDate            -- Use created_at for timestamps
active                 -- Use is_active for booleans
```

---

## Reserved Words

**NEVER use these as column names** (requires quoting):

- user → `app_user`, `user_account`
- order → `customer_order`, `purchase_order`
- group → `user_group`, `permission_group`
- date → `order_date`, `created_date`
- timestamp → `created_at`, `updated_at`

---

## Data Type Suffixes

Use consistent suffixes for clarity:
```sql
_id         -- Primary/Foreign keys: customer_id, product_id
_at         -- Timestamps: created_at, updated_at, deleted_at
_date       -- Dates: birth_date, order_date
_count      -- Integers: order_count, item_count
_amount     -- Money: total_amount, tax_amount
_percent    -- Percentages: discount_percent
_flag       -- Booleans (alternative): active_flag
```

---

## Examples by Industry

### Healthcare
```sql
patient_id
medical_record_number
diagnosis_code
admission_date
discharge_date
is_hipaa_compliant
```

### Finance
```sql
account_number
transaction_amount
routing_number
swift_code
is_suspicious
fraud_score
```

### E-commerce
```sql
product_sku
unit_price
quantity_available
discount_percent
is_taxable
shipping_cost
```

---

[Learn more →](https://www.mdatool.com/blog/database-naming-conventions-complete-style-guide)

