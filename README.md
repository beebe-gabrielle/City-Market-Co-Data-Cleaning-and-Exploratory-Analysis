<img width="760" height="168" alt="image" src="https://github.com/user-attachments/assets/505a986e-df1d-4041-8764-ef999a9a0220" />

<p></p>

# City Market Co. | Sales & Performance Analysis

Tableau Public Dashboard: (__insert link__)

## Tools Used

**Excel** - Data Cleaning, Validation, Calculations

**Tableau** - Data Modeling, Visualization, Dashboard

## Project Overview & Objectives
City Market Co. is a fictional retailer seeking to understand the drivers of sales and profitability across its 20 store locations. Management needs visibility into company-wide growth, product profitability, seasonal trends, and category performance, particularly where high sales volume is not translating into proportional profit.

This analysis aims to translate raw sales data into actionable insights that will address the following business questions posed by management:

* **Is revenue growing over the long term, independent of seasonal spikes?**

* **How consistent is the seasonal pattern across years?**
  
* **Which categories drive both profit and margin?**

* **Which categories carry the highest order values, and which have return-rate problems?**

## Summary of Findings
**Revenue is growing beyond seasonality.** A linear trend line shows baseline monthly revenue rising from roughly $1M to about $1.4M between 2021 and 2025.
  
**The seasonal pattern is consistent.** November and December are the strongest months in every year, and January and February are consistently among the softest.

**Toys and Electronics are the core profit drivers,** pairing above-average profit with above-average margin. Home also narrowly clears both averages.
  
**Beauty and Apparel carry a return-rate problem.** Both pair high revenue with return rates well above the 4.0% company average (8.5% and 7.6%), which puts pressure on the profit they deliver.

## Executive Sales & Performance Dashboard 

<img width="843" height="574" alt="image" src="https://github.com/user-attachments/assets/c1a144dd-9b19-4cbc-9363-c9769c79153b" />


<p></p>

## Headline KPIs (all regions, all years)

| Metric | Value |
|---|---|
| Total Revenue | $73,702,716 |
| Profit Margin | 20.7% |
| Average Order Value | $627.04 |
| Return Rate | 4.0% |

## Dashboard Views

| View | What it shows |
|---|---|
| **Monthly Revenue & Long-Term Growth** | Monthly revenue line with a linear trend line to separate baseline growth from seasonal peaks |
| **Monthly Revenue by Year (heatmap)** | Month × year grid showing recurring year-end (Nov–Dec) peaks, ranging from ~$704K to ~$2.1M |
| **Profitability & Margin by Category** | Profit vs. margin scatter with crosshairs at company averages (20.7% margin / $1.91M profit) |
| **Revenue Contribution by Category** | Ranked revenue by category against the $9.2M category average |
| **Average Order Value by Category** | AOV by category against the $627.04 company baseline |
| **Return Rate by Category** | Return rate by category against the 4.0% company average; categories above average are highlighted |

**Filters:** Region, Category, Year, Month (apply across all views).

## Key Insights

* **Is revenue growing over the long term, independent of seasonal spikes?** Yes. The linear trend line rises steadily from roughly $1M to about $1.4M in monthly revenue between 2021 and 2025, showing baseline growth that is not explained by seasonal peaks alone.

* **How consistent is the seasonal pattern across years?** Very consistent. November and December are the strongest months in every year (reaching about $2.1M), with 2023–2025 showing the highest year-end revenue. January and February are consistently among the softest months.

* **Which categories drive both profit and margin?** Toys and Electronics are the core drivers, landing in the top-right quadrant with above-average profit and margin (vs. the 20.7% margin / $1.91M profit company averages). Home also clears both averages, but only narrowly on profit despite having the highest margin (about 29%). Sports has a strong margin (about 25%) but below-average profit because of its lower revenue. Apparel, Toys, and Electronics together generate roughly 49% of total revenue.

* **Which categories carry the highest order values, and which have return-rate problems?** Toys ($960.30) and Beauty ($797.48) lead on AOV, while Home is lowest at $361.76. Beauty (8.5%), Apparel (7.6%), and Electronics (5.0%) exceed the 4.0% company average return rate. Beauty and Apparel are the biggest concern, since they pair high revenue and order value with high returns.* 

## Recommendations

- Protect and scale **Toys** and **Electronics**, which combine strong profit with strong margin.
- Investigate **Beauty and Apparel returns** (quality, sizing, product descriptions) to recover margin on high-revenue categories.
- Explore ways to grow volume in **Home** and **Sports**, where margins are strong but revenue is low.
- Plan inventory, staffing, and marketing spend around the **Nov–Dec peak**, and consider promotions to lift softer months (Jan–Feb).

## Conclusion

City Market Co. is on a healthy long-term growth path, with revenue climbing steadily beyond the effect of seasonal peaks. Performance is highly seasonal: November and December consistently deliver the strongest results, so planning around the year-end surge is critical.

Profitability is not evenly distributed across the portfolio. Toys and Electronics are the clearest core drivers, while Home and Sports show healthy margins but limited scale. Beauty and Apparel generate substantial revenue and high order values, but their elevated return rates put pressure on the profit they deliver.

The biggest opportunities lie in protecting the strongest categories, reducing returns in high-revenue categories, and building volume where margins are already strong, so that sales growth translates into proportionally stronger profit.

## Data Overview

To ensure accurate analysis, raw transactional records were processed and validated in Excel before being modeled in Tableau. The primary dataset covers retail sales transactions across 20 store locations, tracking order details, product classifications, financial metrics, and customer demographics.

**Data Cleaning & Quality Log:**
* Imputations and Calculations: Imputed missing 'profit' values using 'net_sales_clean - cost_clean', resolved 3,498 missing 'cost' records using 'net_sales_clean - profit_clean', and created a financial_completeness_flag (Complete, Incomplete, Not Usable) to classify record integrity.

* Formatting & Standardization: Standardized text fields, converted numeric strings to clean numeric data types, and addressed negative values in return flags.

**Key Data Attributes:**
* Order Info: order_id, order_date, order_time, channel, customer_segment

* Geography & Store: store_id, region

* Product Hierarchy: category, subcategory

* Financial Metrics: unit_price, quantity, gross_sales, net_sales, cost, profit

* Performance & Data Quality: shipping_days, satisfaction score, return_flag, financial_completeness_flag

**Figure 1: Data Cleaning & Transformation Log Sample**

<img width="1146" height="131" alt="image" src="https://github.com/user-attachments/assets/2b1717a0-1537-4deb-a702-27310b6ad591" />

**Figure 2: Cleaned Dataset Sample**

<img width="1218" height="203" alt="image" src="https://github.com/user-attachments/assets/bfc55982-0e41-4d05-9d20-3640045e3dbe" />

<img width="1288" height="120" alt="image" src="https://github.com/user-attachments/assets/84798493-6f01-49f5-b85b-80e0f72f5d4a" />

## Limitations

* The data is fictional, so findings illustrate the analytical process and are not real business results.
  
* The trend line is linear and shows the overall direction of revenue, not year-to-year changes in growth rate.
  
* The dataset has no return reason codes, so the analysis shows where returns are high but cannot explain why.

* Some cost and profit values were imputed from other fields, so margin figures depend on those calculations.







