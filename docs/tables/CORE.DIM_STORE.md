# Table: `CORE.DIM_STORE`

## Classification

- Type: BASE TABLE
- Classification: DIMENSION (confidence: high)
- Key candidates: `STORE_KEY`

## Description

Store dimension.

## Relationships (inferred)

- Many-to-one to `DIM_GEOGRAPHY` via `GEO_KEY`
- Referenced by facts: `FACT_SALES.STORE_KEY`, `FACT_INVENTORY.STORE_KEY`, `FACT_CAMPAIGN_PERFORMANCE.STORE_KEY`
