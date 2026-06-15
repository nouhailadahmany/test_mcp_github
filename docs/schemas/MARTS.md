# Schema: `MARTS`

## Summary

- Objects: **5 views**
- Columns: **128**
- Constraints present: **No**
- Constraints notes: No constraints returned for this schema (views).

## Views

| View | Type | Classification | Confidence | Key candidates | Notes |
|---|---|---|---|---|---|
| `V_CAMPAIGN_ROI` | VIEW | FACT | medium | *(none)* | Aggregated KPIs (TOTAL_*, ROAS, CTR_PCT, CVR_PCT). |
| `V_CUSTOMER_360` | VIEW | DIMENSION | medium | `CUSTOMER_ID` | Customer profile with aggregated measures (TOTAL_*). |
| `V_INVENTORY_HEALTH` | VIEW | FACT | medium | *(none)* | Inventory measures + derived status. |
| `V_PRODUCT_PERFORMANCE` | VIEW | FACT | medium | `PRODUCT_ID` | Product performance aggregates (NET_REVENUE_EUR, GROSS_PROFIT_EUR, UNIQUE_CUSTOMERS). |
| `V_SALES_PERFORMANCE` | VIEW | FACT | medium | *(none)* | Sales reporting view with measures and breakdown attributes. |

## Relationships

None provided/inferred for this schema.

## Transformation patterns

- **aggregation**: `TOTAL_IMPRESSIONS`, `TOTAL_CLICKS`, `TOTAL_CONVERSIONS`, `TOTAL_SPEND`, `TOTAL_REVENUE_ATTRIBUTED`, `TOTAL_ORDERS`, `TOTAL_UNITS`, `TOTAL_SPEND_EUR`, `AVG_ORDER_VALUE_EUR`, `UNIQUE_CUSTOMERS`
- **date**: `FULL_DATE`, `LAST_ORDER_DATE`, `FIRST_ORDER_DATE`, `YEAR`, `MONTH_NAME`, `QUARTER_NAME`
- **flags**: `IS_ACTIVE`, `IS_NEWSLETTER`, `IS_OUT_OF_STOCK`, `IS_LOW_STOCK`, `IS_RETURNED`
