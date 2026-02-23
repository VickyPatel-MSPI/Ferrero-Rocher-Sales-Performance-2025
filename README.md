# Ferrero Rocher Sales Analysis – 2025

End-to-end retail sales analytics project using Excel and Power BI  

---

### 🎯 Problem Statement

Ferrero Rocher is a premium chocolate product sold globally through multiple retail channels, store formats, and promotional campaigns. Retailers and brand managers need clear visibility into:

- Which geographies, stores and channels are driving the most revenue  
- Which pack sizes (SKUs) perform best and worst  
- Whether promotional campaigns (Diwali, Christmas, Buy 1 Get 1, etc.) actually increase volume and protect margins  
- Seasonal patterns and potential margin erosion risks  

**Business goal**: Provide actionable insights and an interactive dashboard that helps identify top-performing regions/products/promotions and detect underperforming areas that require strategic intervention.

---

### 🗂️ Dataset

**Table Used:** [Ferrero Rocher Sales](https://github.com/VickyPatel-MSPI/Ferrero-Rocher-Sales-Performance-2025/tree/main/Data)

**Source**: Kaggle
**Rows**: ~20,000 transactions  
**Time period**: January 1, 2025 – December 31, 2025  
**Key columns**:

| Column          | Type    | Description                                      | Example / Range                              |
|-----------------|---------|--------------------------------------------------|----------------------------------------------|
| Store           | String  | Retailer name                                    | Tesco, Walmart, Carrefour, Amazon Fresh, …   |
| Country         | String  | Sales country                                    | UK, USA, India, UAE, Canada, Singapore, …    |
| SKU             | String  | Product variant                                  | Ferrero Rocher T3, 16pc, 24pc, 32pc, Collection 15pc |
| Date            | Date    | Transaction date                                 | 2025-01-01 to 2025-12-31                     |
| Channel         | String  | Sales channel                                    | Retail, Wholesale, Online, Offline           |
| Promotion       | String  | Active campaign (None = no promotion)            | Diwali Promo, Buy1Get1, Christmas Promo, …   |
| Units Sold      | Integer | Quantity sold in transaction                     | 10 – 199                                     |
| Unit Price      | Integer | List price per unit                              | 120 – 750                                    |
| Discount        | Float   | Discount rate                                    | 0.00 – 0.50 (0–50%)                          |
| Revenue         | Float   | Net revenue after discount                       | 600 – 149,250                                |
| Margin %        | Integer | Profit margin percentage                         | 25 – 40                                      |
| Margin          | Float   | Profit dollars                                   | 156 – 57,622.5                               |

**Legal Disclaimer:** This resource maintains no official connection to Ferrero Rocher or its parent organization. Every data point has been artificially constructed and purposefully engineered, containing zero reflection of genuine corporate activities, actual market performance, or authentic financial metrics. This material serves exclusively academic purposes, supporting activities such as analytical skill-building, interactive visualization projects, business metric evaluation, and professional work samples for career advancement.

---

### 📌 Analysis & KPI Computation

**Tools used**  
• Excel – data cleaning & validation   
• Power BI – KPI measures, visuals & interactivity

**Core KPIs calculated**:

- Total Revenue  
- Total Units Sold  
- Average Units per Transaction  
- Average Selling Price (ASP)  
- Average Discount %  
- Average Margin %  
- Total Margin $   
- Revenue Share % by Country / Store / SKU / Channel  
- Monthly / Quarterly revenue & units trend  
- Top N & Bottom N rankings (SKU, Store, Promotion)

All important metrics are implemented as reusable DAX measures in Power BI.

---

### 📊 Power BI Dashboards

**Report contains 6 main pages**:

1. **Executive Overview**  
   KPIs • Revenue by Country (donut) • Top Stores (bar) • Monthly trend (combo)

2. **Time & Trend Analysis**  
   Stacked area – Revenue by Promotion over months  
   Dual-axis line – Price vs Discount trend  
   Clustered column – Units by Channel & Month

3. **SKU Performance**  
   Treemap – Revenue share by SKU  
   Stacked bar – Units by SKU & Channel  
   Scorecard matrix (Revenue, Units, Margin %, Discount %)

4. **Promotion Effectiveness**  
   Clustered column – Revenue & Margin % by Promotion  
   Bar chart – Units Sold Lift % vs No Promotion baseline  
   Scatter – Revenue vs Avg Discount by Promotion

5. **Geographic & Channel Breakdown**  
   Filled map – Revenue by Country  
   Stacked column – Revenue by Country & Channel  
   Matrix heatmap – Country × Channel revenue

6. **Margin & Profitability**  
   Gauge & distribution visuals – Margin %  
   Stacked bar – Margin $ by SKU & Promotion  
   Scatter – Revenue vs Margin $

All pages include cross-filtering slicers: Country, Channel, Promotion, SKU, Date range.

---

### 🔍 Key Insights

(Extracted from the actual dataset analysis)

- **Top 5 revenue countries**: Singapore > USA > Canada > UK > UAE  
- **Best performing SKU**: Ferrero Rocher 32pc – highest average revenue per transaction  
- **Worst performing SKU (volume)**: Ferrero Rocher T3 – lowest average units & revenue  
- **Promotion impact on volume**: All listed promotions showed **negative units lift** compared to no-promotion baseline  
  → Christmas Promo performed best (−0.6%)  
  → NewYear Sale performed worst (−2.8%)  
- **Margin insight**: Wholesale channel generally preserves higher margin % than Retail or Online  
- **Seasonality**: Clear revenue peaks in October–December (Diwali + Christmas + New Year)  
- **Discount pressure**: Higher discounts correlate with slightly lower average units per transaction (possible small-basket / price-sensitive buyer attraction)

---

### 🎯 Conclusion

The 2025 Ferrero Rocher sales data reveals strong geographic concentration (Singapore, North America, UK, UAE) and SKU preference toward larger pack sizes (32pc). However, promotional campaigns — while likely increasing transaction count — appear to attract lower average basket sizes, resulting in **negative volume lift** compared to non-promotional periods.

**Recommended next steps**:

- Re-evaluate promotion mechanics (focus on margin-accretive offers rather than deep discounts)  
- Strengthen presence in high-margin channels (Wholesale)  
- Push larger pack SKUs more aggressively in key markets  
- Run A/B tests on new promotion structures in 2026

This project demonstrates full-cycle analytics: data cleaning → SQL exploration → interactive BI reporting.

Feel free to fork, extend or use it as inspiration for your own retail / FMCG analysis work.

⭐ If you find it useful – give the repo a star!

Questions / suggestions → open an issue.

---

**Contributions**

Explore the Power BI dashboard for interactive visualizations: [Ferrero Rocher Sales Performance](https://github.com/VickyPatel-MSPI/Ferrero-Rocher-Sales-Performance-2025/tree/main/Power%20BI)

Explore the Excel word file for query and data analysis: [Ferrero Rocher Sales](https://github.com/VickyPatel-MSPI/Ferrero-Rocher-Sales-Performance-2025/tree/main/Data)

---
