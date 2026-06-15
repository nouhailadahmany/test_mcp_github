# Table: `CORE.FACT_SALES`

- Type: BASE TABLE
- Classification: FACT (confidence: high)
- Key candidates: `SALE_KEY`
- Notes: Sales measures + multiple dimension keys; has return fields.

## Relationships (dimension links)

- Many-to-one to `CORE.DIM_DATE` via `DATE_KEY` (confidence: medium)
- Many-to-one to `CORE.DIM_DATE` via `RETURN_DATE_KEY` (confidence: low; role-playing mapping inferred)
- Many-to-one to `CORE.DIM_CUSTOMER` via `CUSTOMER_KEY` (confidence: medium)
- Many-to-one to `CORE.DIM_PRODUCT` via `PRODUCT_KEY` (confidence: medium)
- Many-to-one to `CORE.DIM_STORE` via `STORE_KEY` (confidence: medium)
- Many-to-one to `CORE.DIM_GEOGRAPHY` via `GEO_KEY` (confidence: medium)
- Many-to-one to `CORE.DIM_CAMPAIGN` via `CAMPAIGN_KEY` (confidence: medium)
- Many-to-one to `CORE.DIM_PROMOTION` via `PROMO_KEY` (confidence: medium)
