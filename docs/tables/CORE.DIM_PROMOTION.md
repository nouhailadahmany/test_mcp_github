# Table: `CORE.DIM_PROMOTION`

- Type: BASE TABLE
- Classification: DIMENSION (confidence: high)
- Key candidates: `PROMO_KEY`
- Notes: Promotion dimension.

## Relationships

- Many-to-one to `CORE.DIM_CAMPAIGN` via `CAMPAIGN_KEY` (confidence: medium; mapping inferred by naming).
