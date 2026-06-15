# Database Documentation

Generated documentation for the database schemas and tables:

- [`docs/overview.md`](docs/overview.md)
- Schemas:
  - [`AUDIT`](docs/schemas/AUDIT.md)
  - [`CORE`](docs/schemas/CORE.md)
  - [`MARTS`](docs/schemas/MARTS.md)
  - [`STAGING`](docs/schemas/STAGING.md)

---

## Structure

- `docs/overview.md`: high-level overview of the database and schema flow.
- `docs/schemas/<schema>.md`: per-schema summary (tables/views, patterns, relationships when available).
- `docs/tables/<schema>.<table>.md`: per-table/view documentation (classification, keys, notes, inferred relationships).

---

## Notes on constraints

In multiple schemas, `KEY_COLUMN_USAGE` was not accessible, so some FK column mappings are **inferred by naming conventions** even when FK constraints are known to exist.
