# Table: `AUDIT.LOAD_LOG`

## Classification

- Type: BASE TABLE
- Classification: FACT (confidence: medium)
- Key candidates: `LOG_ID`

## Description

Pipeline load metrics (rows_, timestamps, status).

## Common columns/patterns

- Metrics: `ROWS_EXTRACTED`, `ROWS_LOADED`, `ROWS_REJECTED`, `ROWS_UPDATED`
- Timestamps: `START_TIME`, `END_TIME`, `CREATED_AT`
- Keys: `LOG_ID`, `BATCH_ID`

## Relationships

None provided.
