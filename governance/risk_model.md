# RISK MODEL — SAFE COSMETICS MARKETPLACE

## Purpose

The risk model determines how products and sellers are evaluated, routed, and approved.
It ensures that high-risk items receive human oversight and low-risk items move efficiently through automated checks.

---

## I. Risk Inputs

### A. Product-Level Inputs

| Factor | Description | Score Range |
|-------|-------------|-------------|
| **Category Risk** | Cleansers vs acids vs devices | 0–30 |
| **Ingredient Risk** | Banned, restricted, concentration, pH | 0–30 |
| **Documentation Completeness** | CPSR, PIF, labels, RP | 0–15 |
| **Claim Risk** | Medical, borderline, misleading | 0–15 |
| **Packaging Risk** | Missing warnings, incorrect INCI | 0–10 |

**Product subtotal:** 0–100

---

### B. Seller-Level Inputs

| Factor | Description | Score Range |
|-------|-------------|-------------|
| **Seller Tier** | Tier 1–3 | 0–20 |
| **History** | Rejections, suspensions, incidents | 0–20 |
| **Documentation Quality** | Accuracy, timeliness | 0–10 |
| **Behavioural Risk** | Attempts to bypass rules | 0–10 |

**Seller subtotal:** 0–60

---

## II. Combined Risk Score

$$
\text{Total Risk} = \text{Product Risk} + \text{Seller Risk}
$$

**Range:** 0–160

---

## III. Risk Bands & Required Actions

| Total Score | Band | Action |
|-------------|------|--------|
| **0–40** | Low | Auto-approve if compliant |
| **41–90** | Medium | Automated + spot human review |
| **91–130** | High | Mandatory human review |
| **131–160** | Critical | Auto-block + escalate |

---

## IV. Risk Rationale Output

Every risk score produces:

- numerical score
- band
- top contributing factors
- recommended action
- human-readable explanation

Example:

> “High risk due to restricted ingredient concentration, borderline claims, and seller Tier 1 status.”

---

## V. Continuous Learning

The model updates based on:

- incident reports
- regulatory changes
- seller behaviour
- new ingredient science
