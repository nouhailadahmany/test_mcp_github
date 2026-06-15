# Table: `CORE.FACT_CAMPAIGN_PERFORMANCE`

## Classification

- Type: BASE TABLE
- Classification: FACT (confidence: high)
- Key candidates: `PERF_KEY`

## Description

Campaign performance fact table with many metrics and multiple dimension keys.

## Relationships (inferred)

- Many-to-one to `DIM_DATE` via `DATE_KEY`
- Many-to-one to `DIM_CAMPAIGN` via `CAMPAIGN_KEY`
- Many-to-one to `DIM_STORE` via `STORE_KEY`
- Many-to-one to `DIM_GEOGRAPHY` via `GEO_KEY`
