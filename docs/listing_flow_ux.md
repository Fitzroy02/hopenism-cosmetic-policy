# Listing Flow UX

This document defines a concise five-step listing flow.

## Step 1 — Product Basics

- **Fields:** product name, category, sub-category, target audience (adult/child), region of sale.
- **Guardrail:** category selection auto-sets risk baseline.

## Step 2 — Ingredients & Documentation

- **Inputs:** full INCI list, concentrations (where relevant), pH (if applicable).
- **Uploads:** CPSR, PIF, label artwork.
- **Live feedback:** ingredient scanner runs with inline warnings/errors.

## Step 3 — Claims & Positioning

- **Fields:** marketing claims, usage instructions, warnings.
- **Guardrail:** claim classifier flags medical/borderline language in real time.

## Step 4 — Compliance Summary

- **Panel:**
  - Ingredient check: ✅/❌
  - Claims check: ✅/⚠️
  - Label check: ✅/❌
  - Documentation: ✅/❌
- **Outcome:** ready for submission or issues to resolve.

## Step 5 — Submission & Review

- **Status path:** pending automated checks → auto-approve or route to human review (high-risk).
- **Traceability:** listing ID, timestamp, seller ID.
