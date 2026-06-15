# Overview

This documentation describes four schemas and their tables/views, classifications (fact vs dimension), inferred keys, detected transformation patterns, and (where available) relationships.

## Schemas

| Schema | Tables/Views | Columns | Constraints | Notes |
|---|---:|---:|---|---|
| `AUDIT` | 2 | 30 | Yes | PKs detected; PK/FK column mappings unavailable (`KEY_COLUMN_USAGE` not accessible). |
| `CORE` | 10 | 223 | Yes | PK/FK constraints detected; FK column mappings inferred by naming. |
| `MARTS` | 5 | 128 | No | Views only; no constraints returned. |
| `STAGING` | 3 | 46 | Yes | PKs detected; PK column mappings not confirmed beyond naming. |

## Model shape (high-level)

- **`STAGING`**: raw landing tables (TEXT-heavy measures), with ingestion/audit columns and `RAW_JSON`.
- **`CORE`**: curated star-schema style model with multiple dimensions and facts.
- **`MARTS`**: reporting/analytics views with aggregated KPIs and customer/product rollups.
- **`AUDIT`**: operational auditing and quality/load logging tables.

## Common transformation patterns

- **Keys**: `*_KEY`, `*_ID`, `BATCH_ID`, `RAW_ID`
- **Dates/Timestamps**: `FULL_DATE`, `START_DATE`, `END_DATE`, `*_TIME`, `*_AT`, `*_DATE_KEY`
- **Flags**: `IS_*`
- **Metrics/Aggregations**: `TOTAL_*`, `ROWS_*`, and KPI fields such as `ROAS`, `CTR`, `CVR`
