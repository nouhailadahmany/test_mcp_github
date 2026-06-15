# Table: `CORE.FACT_INVENTORY`

## Classification

- Type: BASE TABLE
- Classification: FACT (confidence: high)
- Key candidates: `INVENTORY_KEY`

## Description

Inventory fact table with measures and multiple dimension keys.

## Relationships (inferred)

- Many-to-one to `DIM_DATE` via `DATE_KEY`
- Many-to-one to `DIM_PRODUCT` via `PRODUCT_KEY`
- Many-to-one to `DIM_STORE` via `STORE_KEY`
- Many-to-one to `DIM_GEOGRAPHY` via `GEO_KEY`
