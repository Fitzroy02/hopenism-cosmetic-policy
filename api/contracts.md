# MARKETPLACE API CONTRACTS (v1)

Base path:
`/api/v1`

All endpoints return:

```json
{
  "status": "success|error",
  "data": {},
  "errors": []
}
```

---

## I. Seller Endpoints

### POST /sellers

Register a new seller.

**Request:**

```json
{
  "name": "string",
  "business_registration": "string",
  "address": "string",
  "email": "string"
}
```

**Response:**

```json
{
  "seller_id": "uuid",
  "tier": 1
}
```

---

### GET /sellers/{id}

Retrieve seller profile.

**Response:**

```json
{
  "seller_id": "uuid",
  "tier": 2,
  "compliance_score": 87,
  "documents": {
    "cpsr": "verified",
    "pif": "pending"
  }
}
```

---

## II. Product Endpoints

### POST /products

Create a product draft.

**Request:**

```json
{
  "seller_id": "uuid",
  "name": "string",
  "category": "string"
}
```

**Response:**

```json
{
  "product_id": "uuid",
  "status": "draft"
}
```

---

### PATCH /products/{id}

Update product details.

**Request:**

```json
{
  "ingredients": [...],
  "claims": [...],
  "documentation": {...}
}
```

---

### POST /products/{id}/submit

Submit for review.

**Response:**

```json
{
  "product_id": "uuid",
  "status": "pending_review"
}
```

---

## III. Compliance Endpoints

### POST /compliance/scan

Run automated checks.

**Request:**

```json
{
  "ingredients": [...],
  "claims": [...],
  "label": {...}
}
```

**Response:**

```json
{
  "ingredient_flags": [...],
  "claim_flags": [...],
  "label_flags": [...],
  "overall_status": "pass|fail"
}
```

---

## IV. Risk Endpoints

### GET /risk/products/{id}

Retrieve risk score.

**Response:**

```json
{
  "risk_score": 72,
  "risk_band": "medium",
  "rationale": [
    "Restricted ingredient concentration",
    "Seller Tier 1"
  ]
}
```

---

## V. Moderation Endpoints

### POST /moderation/products/{id}/actions

Moderate a listing.

**Request:**

```json
{
  "action": "approve|reject|suspend",
  "reason": "string"
}
```
