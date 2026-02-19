# CLAIMS CLASSIFICATION MODEL

## Purpose

To classify product claims into safe, borderline, or prohibited categories.

---

## I. Claim Categories

### A. Safe Claims (Allowed)

- Cosmetic effects
- Sensory descriptions
- Non-functional marketing language

Examples:

- “Moisturises the skin”
- “Leaves skin feeling soft”
- “Lightweight texture”

---

### B. Borderline Claims (Flagged)

Require evidence and may be rejected.

Examples:

- “Reduces acne”
- “Repairs skin barrier”
- “Anti-inflammatory”

---

### C. Prohibited Claims

Medical or therapeutic.

Examples:

- “Treats eczema”
- “Heals psoriasis”
- “Cures fungal infections”

---

## II. Classification Logic

### Step 1 — Keyword Scan

- Medical terms → prohibited
- Functional biological terms → borderline
- Cosmetic terms → safe

### Step 2 — Contextual Analysis

- “Helps reduce the appearance of” → borderline
- “Clinically proven to treat” → prohibited

### Step 3 — Evidence Requirement

Borderline claims require:

- study data
- justification
- RP approval

### Step 4 — Final Output

```json
{
  "claim": "string",
  "classification": "safe|borderline|prohibited",
  "rationale": "string",
  "required_action": "none|provide evidence|remove claim"
}
```
