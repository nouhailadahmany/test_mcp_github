# Table: `CORE.DIM_CUSTOMER`

- Type: BASE TABLE
- Classification: DIMENSION (confidence: high)
- Key candidates: `CUSTOMER_KEY`
- Notes: SCD-like columns (EFF_START_DATE, EFF_END_DATE, IS_CURRENT).

## Relationships

- Many-to-one to `CORE.DIM_GEOGRAPHY` via `GEO_KEY` (confidence: medium; mapping inferred by naming).
