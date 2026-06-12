# Corporate Sales Performance Analysis — Power BI

> A single-page enterprise dashboard analyzing 22.5K orders and $87.7M in revenue. Covers fulfillment efficiency, channel behavior, regional distribution, and financial performance across 2011–2014.

---

## Key Metrics

| KPI | Value |
|-----|-------|
| Total Orders | 22,540 |
| Total Due (gross revenue) | $87.70M |
| Sub Total (product revenue) | $78.18M |
| Total Tax | $7.26M |
| Total Freight | $2.27M |
| Avg. Delivery Time | 12 days |

---

## Dashboard

![Sales Analysis Dashboard](Image/sales%20analysis%20dashboard%20power.jpg)

---

## Visual breakdown

### Filtering (top pane)
Dynamic drop-down slicers for Date, Product, and Regional Group — all cross-filter the entire data model simultaneously.

### Behavioral insights

| Visual | Finding |
|--------|---------|
| Online vs. offline orders (donut) | 87.76% of orders are offline (19.75K); online accounts for 12.24% (2.79K) — significant brick-and-mortar dependency |
| Fulfillment trends by year (line chart) | Orders, delivered orders, and shipped orders tracked 2011–2014; significant scaling peak in 2013 |
| Weekday vs. weekend orders (pie) | 71.63% of purchases happen on weekdays — weekend promotions may be an untapped lever |

### Product & regional performance

| Visual | Purpose |
|--------|---------|
| Orders by category (stacked bar) | Accessories and Bikes are the primary volume drivers, followed by Clothing and Components |
| Orders by group (Azure Map) | High-density sales clusters in North America and Europe |
| Total Due & orders by business entity (combo chart) | Dual-axis bar + line correlating vendor revenue against order volume — identifies top-performing partners |

---

## Data Model & Technical Specs

**Architecture:** Star schema separating fact and dimension tables

```
Fact: Sales Transactions
Dimensions: Date · Customer · Product · Geography
```

**DAX highlights:**
- Time intelligence for year-over-year trend analysis
- Average delivery duration metric
- Conditional segmentation for weekday vs. weekend behavior

**Platform:** Power BI Desktop / Power BI Service  
**Map integration:** Microsoft Azure Maps

---

## Insights this dashboard surfaces

- Offline orders dominate — understanding why online lags could unlock significant growth
- 2013 was the peak fulfillment year; the dashboard helps identify what drove that and whether it's repeatable
- Weekday concentration in purchasing suggests B2B buyer behavior may be significant in the mix
- Top business entities by revenue vs. order count reveal which partners are high-value vs. high-volume
