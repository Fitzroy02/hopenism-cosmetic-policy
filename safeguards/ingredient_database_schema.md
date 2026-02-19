# INGREDIENT DATABASE SCHEMA

A structured database for ingredient safety, regulatory status, and concentration limits.

---

## I. Ingredient Table

| Field | Type | Description |
|-------|------|-------------|
| ingredient_id | UUID | Unique identifier |
| inci_name | String | Official INCI name |
| cas_number | String | Chemical identifier |
| category | Enum | Active, preservative, fragrance, colourant, etc. |
| banned | Boolean | True if banned |
| restricted | Boolean | True if restricted |
| max_concentration | Decimal | Legal limit |
| min_pH | Decimal | Minimum safe pH |
| max_pH | Decimal | Maximum safe pH |
| allergen | Boolean | True if allergen |
| nano | Boolean | True if nanomaterial |
| notes | Text | Additional regulatory notes |

---

## II. Regulatory Source Table

| Field | Type | Description |
|-------|------|-------------|
| source_id | UUID | Unique identifier |
| ingredient_id | UUID | Linked ingredient |
| regulation | String | e.g., “EU Annex III” |
| reference | String | Clause or annex number |
| jurisdiction | Enum | UK, EU |
| last_updated | Date | Regulatory update date |

---

## III. Concentration Rules Table

| Field | Type | Description |
|-------|------|-------------|
| rule_id | UUID | Unique identifier |
| ingredient_id | UUID | Linked ingredient |
| product_type | String | e.g., “rinse-off”, “leave-on” |
| max_concentration | Decimal | Allowed limit |
| conditions | Text | e.g., “Not for use on children under 3” |
