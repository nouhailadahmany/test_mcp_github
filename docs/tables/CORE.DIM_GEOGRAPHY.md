# Table: `CORE.DIM_GEOGRAPHY`

## Classification

- Type: BASE TABLE
- Classification: DIMENSION (confidence: high)
- Key candidates: `GEO_KEY`

## Description

Geography dimension.

## Relationships (inferred)

- Referenced by `DIM_CUSTOMER.GEO_KEY`
- Referenced by `DIM_STORE.GEO_KEY`
- Referenced by facts: `FACT_SALES.GEO_KEY`, `FACT_INVENTORY.GEO_KEY`, `FACT_CAMPAIGN_PERFORMANCE.GEO_KEY`
