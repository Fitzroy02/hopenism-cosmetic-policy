# Marketplace API Structure

Base path: `/api/v1`

All endpoints are auditable with user, timestamp, action, and payload snapshot.

## Sellers

- `POST /sellers` — register seller.
- `GET /sellers/{id}` — seller profile, tier, compliance score.
- `GET /sellers/{id}/documents` — documentation status.

## Products

- `POST /products` — create listing draft.
- `GET /products/{id}` — product details, risk level, compliance report.
- `GET /products?seller_id=` — list seller products.
- `PATCH /products/{id}` — update listing.
- `POST /products/{id}/submit` — submit for review.

## Compliance

- `POST /compliance/scan` — run ingredient, claim, and label checks.
- `GET /compliance/products/{id}` — compliance summary and flags.

## Risk

- `GET /risk/products/{id}` — risk score and rationale.
- `GET /risk/sellers/{id}` — seller risk profile.

## Moderation

- `POST /moderation/products/{id}/actions` — suspend/reject/approve with reason.
