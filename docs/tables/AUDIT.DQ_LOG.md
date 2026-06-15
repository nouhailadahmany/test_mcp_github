# Table: `AUDIT.DQ_LOG`

## Classification

- Type: BASE TABLE
- Classification: FACT (confidence: medium)
- Key candidates: `DQ_LOG_ID`

## Description

Log/metrics table with counts/rates/timestamps.

## Common columns/patterns

- Metrics: `ROWS_CHECKED`, `ROWS_FAILED`, `FAILURE_RATE`
- Timestamps: `CREATED_AT`, `CHECKED_AT`, `START_TIME`, `END_TIME`
- Keys: `DQ_LOG_ID`, `BATCH_ID`

## Relationships

None provided.
