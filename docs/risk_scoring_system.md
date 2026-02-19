# Risk Scoring System

This system produces a score from 0–100 to determine review and enforcement pathways.

## Inputs

### Product Factors

- Category risk (for example cleanser vs peel).
- Ingredient profile (banned/restricted, concentration, pH).
- Documentation completeness.
- Claims risk (medical/borderline).

### Seller Factors

- Tier (1–3).
- History (rejections, suspensions, adverse events).
- Documentation quality and timeliness.

## Scoring Bands

- **0–25:** low risk → automated approval if compliant.
- **26–60:** medium risk → automated checks plus spot human review.
- **61–100:** high risk → mandatory human review and possible pre-emptive block.

## Outputs

- Risk score (0–100).
- Risk band (Low/Medium/High).
- Human-readable rationale.
- Recommended action (approve, review, block).
