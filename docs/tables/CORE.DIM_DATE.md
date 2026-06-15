# Table: `CORE.DIM_DATE`

## Classification

- Type: BASE TABLE
- Classification: DIMENSION (confidence: high)
- Key candidates: `DATE_KEY`

## Description

Calendar dimension.

## Relationships (inferred)

- Referenced by `FACT_SALES.DATE_KEY`
- Referenced by `FACT_SALES.RETURN_DATE_KEY` (role-playing)
- Referenced by `FACT_INVENTORY.DATE_KEY`
- Referenced by `FACT_CAMPAIGN_PERFORMANCE.DATE_KEY`
