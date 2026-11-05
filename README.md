# 🛒 Retail Sales & Store Performance Dashboard (Power BI)

An interactive **two-page Power BI dashboard** analysing **10,000 retail transactions in 2025** across **30 stores in 8 Australian states**. It gives executives a single view of revenue, profit, customer behaviour, promotions and store operations.

---

## 📌 Project Overview

| | |
|---|---|
| **Goal** | Track financial performance and identify which stores, products, channels and promotions drive profit |
| **Data** | `FMH_Dataset.csv`: 10,000 transactions × 35 columns (Jan–Dec 2025) |
| **Tool** | Microsoft Power BI Desktop |
| **Features** | KPI cards, waterfall-style breakdown, trend area chart, decomposition tree, matrix, treemap, slicers for drill-down |

### Headline KPIs

| Total revenue | Cost of goods | Gross profit | Gross margin | Return rate | Avg customer rating | Stockout alerts |
|---|---|---|---|---|---|---|
| **$208.3K** | $141.5K | **$62.0K** | **29.8%** | 1.5% | 4.17 / 5 | 373 |

---

## 📂 Repository Structure

```
.
├── FMH_Dashboard.pbix          # Power BI report file
├── data/
│   └── FMH_Dataset.csv         # Source dataset
├── images/
│   ├── page1_executive_overview.png
│   └── page2_store_operations.png
├── dashboard_powerbi.pdf       # PDF export of the dashboard
└── README.md
```

---

## 🗂️ Dataset

Each row is one transaction line. The 35 columns fall into these groups:

| Group | Columns |
|---|---|
| **Time** | Transaction_Date, Transaction_Time, Month, Quarter, Day_of_Week, Weekend_Flag |
| **Store** | Store_ID, Store_Name, City, State, Location_Type (Metro / Regional / Suburban), Store_Size |
| **Product** | Product_ID, Product_Name, Category (10), Subcategory |
| **Financials** | Unit_Price, Unit_Cost, Quantity, Discount_Pct, Sales_Revenue, Cost_of_Goods, Gross_Profit, Profit_Margin_Pct |
| **Promotion** | Promotion_Type (No Promotion, Weekly Special, Member Special, Bundle Offer, Clearance) |
| **Customer** | Loyalty_Tier, Customer_Age_Group, Payment_Method, Customer_Rating |
| **Operations** | Sales_Channel, Fulfilment_Method, Return_Flag, Stockout_Flag, Weather |

---

## 📊 Dashboard Pages

### Page 1: Executive Financial & Temporal Overview
![Executive overview](images/page1_executive_overview.png)

| Visual | What it shows |
|---|---|
| Financial waterfall breakdown | Revenue ($208.3K) → cost of goods ($141.5K) → gross profit ($62.0K), a **29.8% margin** |
| Revenue & gross profit trend | Monthly trend for 2025, with a clear **peak in December** (~$23K revenue) |
| Revenue by sales channel | **In-store 80%** vs online 20% |
| KPI cards | Average return rate 1.5%, average customer rating 4.17 |
| Transactions by time period | Hourly trading pattern: steady through the day, dropping sharply after 7 pm |
| Transactions by promotion | 47% of transactions have no promotion. Weekly and member specials lead among promotions. |
| Top 10 products by gross profit | Led by Salmon Fillet 400g, Sunscreen SPF50 and Tea Bags 100pk |

**Slicers:** Customer age group, Weather, Quarter

### Page 2: Store & Geographic Operations
![Store operations](images/page2_store_operations.png)

| Visual | What it shows |
|---|---|
| Sales revenue by state | **NSW 42%**, QLD 18%, VIC 17%. Smaller states make up the rest. |
| Top 5 / bottom 5 stores by gross profit | Parramatta, Liverpool and Castle Hill lead. Darwin, Launceston and Townsville trail. |
| Total stockout alerts | 373 transactions flagged with a stockout |
| Returns by state | Returns are concentrated in NSW, in line with its sales volume |
| Revenue decomposition tree | Drill from total → store → category → subcategory |
| Location & size performance matrix | Metro stores generate **$110K revenue / $32.7K profit**, more than regional and suburban combined |
| Gross profit by fulfilment method | Store purchase dominates (~$53.8K). Home delivery and click & collect earn about $4K each. |

**Slicers:** State, Location type, Store size

---

## 💡 Key Insights

1. **Sales are concentrated in NSW and Metro stores.** Together they account for the bulk of revenue and profit, so they are the core of the business.
2. **Physical stores dominate.** In-store sales make up 80% of revenue, and store purchases generate most of the profit, so online is a growth opportunity.
3. **There is a strong year-end peak.** December revenue is the highest of the year, so inventory and staffing should be planned for Q4.
4. **Fresh and everyday items drive profit.** Salmon, sunscreen and tea bags lead gross profit, and they are good candidates for featured promotions.
5. **Operational risks to watch.** 373 stockouts point to lost sales, and the bottom-performing regional stores (Darwin, Launceston) may need review.
6. **Customers are satisfied.** A 4.17 average rating and a low 1.5% return rate show healthy service quality.

---


---

## 👤 Author

**Van Phong Nguyen**
📧 phongnguyenvan97dn@gmail.com
