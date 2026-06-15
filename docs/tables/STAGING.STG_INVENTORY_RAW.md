# Table: `STAGING.STG_INVENTORY_RAW`

## Classification

- Type: BASE TABLE
- Classification: FACT (confidence: low)
- Key candidates: `RAW_ID`

## Description

Raw landing table; measures stored as TEXT; includes `RAW_JSON` and ingestion/process columns.

## Common columns/patterns

- Raw payload: `RAW_JSON`
- Ingestion audit: `SOURCE_SYSTEM`, `SOURCE_FILE`, `BATCH_ID`, `LOAD_TIMESTAMP`, `ERROR_MESSAGE`
- Flags: `IS_PROCESSED`
- Dates as text: `SNAPSHOT_DATE`

## Relationships

None provided.
