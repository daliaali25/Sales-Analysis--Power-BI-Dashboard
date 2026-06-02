# Corporate Sales Performance Analysis (Power BI)

A comprehensive, interactive Power BI dashboard designed to analyze and evaluate corporate sales performance, order fulfillment cycles, and financial metrics. This enterprise-grade solution transforms raw sales transactions into actionable strategic insights, focusing on revenue health, operational efficiency, and regional distribution.

🔗 [View Interactive Dashboard on Power BI Service](https://app.powerbi.com/groups/7a8be7ff-51f5-4f41-8be8-521c59d2e4cb/reports/e01b3e52-beec-4c6f-8f43-69b901528755/e3e3b64934be1932d75e?experience=power-bi)

---

## 📊 Business Intelligence & Dashboard Overview

This single-page analytical system leverages an elegant, desaturated sage-green visual theme with a structured grid layout. It integrates core financial KPIs with precise operational and behavioral breakdowns to give stakeholders an immediate, holistic view of performance.

### Key Performance Indicators (KPIs):
*   **Total Orders (Orders):22.54K total transactions processed.
Total Financial Volume:
    Total Due:$87.70M (Gross Revenue including taxes and logistics).
    Sub Total: $78.18M (Core Product Revenue).
Operational Costs:
    Total Tax:$7.26M accumulated tax expenses.
    Total Freight:$2.27M total shipping and logistics costs.
Fulfillment Efficiency:y12 Dayson average to successfully deliver an order.

---

## 🖥️ Dashboard Architecture & Visual Analytics


![Sales Analysis Dashboard](Image/sales%20analysis%20dashboard%20power.jpg)

### 1. Advanced Filtering & Slicers (Top Pane)
*   Equipped with dynamic drop-down slicers DateteProductct, Regional Groupup to allow cross-filtering across the entire data model.

### 2. Behavioral & Time-Based Insights
Orders by OnlineOrderFlag (Donut Chart): Tracks customer acquisition channels, showing that the vast majority of orders 87.76% / 19.75K are driven by offline/store transactions, while online sales represent 12.24% / 2.79K9K.
Fulfillment Trends by Year (Line Chart):A continuous timeline comparison track Orders, Delivered Orders, and Shipped Orders from 2011 to 2014, showing a significant scaling peak in 2013.
#Orders by IsWeekend (Pie Chart):Breaks down purchasing habits based on weekday vs. weekend active 71.63% Weekdays 28.37% Weekends.

### 3. Product & Regional Performance
#Orders by Category (Stacked Bar Chart):Ranks product segments by volume, highlight Accessories Bikeses as the primary volume drivers, followed by *Clothing* and *Components*.
Orders by Group (Geographic Map): Uses Microsoft Azure Map integration to visualize global sales concentration, pointing out high-density clusters in North America and Europe.
Total Due & Orders by BusinessEntityID (Combo Chart): A sophisticated dual-axis chart (Bar + Line) that correlates vendor/business entity revenue generation (Total Due) against their absolute order volumes (Orders), identifying top-performing business partners.

---

## 🛠️ Data Engineering & Modeling Specs

Technology Stack: Power BI Desktop / Power BI Service.
Data Modeling: Implemented a Star Schema separating Fact tables (Sales Transactions) from Dimension tables (Date, Customer, Product, Geography).
DAX Calculations: Utilized advanced DAX for custom explicit measures (Time Intelligence for yearly trends, average delivery duration metrics, and conditional segmentation for weekends).
UI/UX Design: High-end report interface utilizing modern shadow containers, customized tooltips, and a cohesive corporate color palette to avoid visual clutter.

---

## 🚀 How to Interact with the Dashboard

1. Click [Power BI Service Link](https://app.powerbi.com/groups/7a8be7ff-51f5-4f41-8be8-521c59d2e4cb/reports/e01b3e52-beec-4c6f-8f43-69b901528755/e3e3b64934be1932d75e?experience=power-bi)
2. Use the Slicers at the top to isolate specific time frames or product categories.
3. Hover over visual elements to trigger interactive tooltips, or click on any chart segment (e.g., "Bikes" or "North America") to cross-highlight related metrics across the entire dashboard page.