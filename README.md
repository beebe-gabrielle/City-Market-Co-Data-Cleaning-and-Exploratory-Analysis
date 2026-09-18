<img width="760" height="168" alt="image" src="https://github.com/user-attachments/assets/505a986e-df1d-4041-8764-ef999a9a0220" />

<p></p>

# City Market Co. | Sales & Product Performance Analysis

Tableau Public Dashboard: (__insert link__)

## Tools Used

**Excel** - Data Cleaning, Validation, Calculations

**Tableau** - Data Modeling, Visualization, Dashboard

## Project Overview & Objectives
City Market Co. is a fictional retailer seeking to understand the drivers of sales and profitability across its 20 store locations. Management needs visibility into regional and city-level performance, product profitability, seasonal trends, and areas where sales volume is not translating into proportional profit. 

This analysis aims to translate raw sales data into actionable insights that will address the following business questions posed by management:

* **Where are our strongest and weakest markets across regions and cities?**

* **How is company perfomance evolving YoY?**

* **Which seasonal cycles most affect sales and profitability?**

* **Which product areas drive margin growth, and which erode profitablity?**

## Data Overview

To ensure accurate analysis, raw transactional records were processed and validated in Excel before being modeled in Tableau. The primary dataset covers retail sales transactions across 20 store locations, tracking order details, product classifications, financial metrics, and customer demographics.

**Data Cleaning & Quality Log:**
* Imputations and Calculations: Imputed missing 'profit' values using 'net_sales_clean - cost_clean', resolved 3,498 missing 'cost' records using 'net_sales_clean - profit_clean', and created a financial_status_flag (Complete, Incomplete, Not Usable) to classify record integrity.

* Formatting & Standardization: Standardized text fields, converted numeric strings to clean numeric data types, and addressed negative values in return flags.

**Key Data Attributes:**
* Order Info: order_id, order_date, order_time, channel, customer_segment

* Geography & Store: store_id, region

* Product Hierarchy: category, subcategory

* Financial Metrics: unit_price, quantity, gross_sales, net_sales, cost, profit

* Performance & Data Quality: shipping_days, satisfaction score, return_flag, financial_completeness_flag

**Figure 1: Data Cleaning & Transformation Log**

<img width="1146" height="131" alt="image" src="https://github.com/user-attachments/assets/2b1717a0-1537-4deb-a702-27310b6ad591" />

**Figure 2: Cleaned Dataset Sample**

<img width="1218" height="203" alt="image" src="https://github.com/user-attachments/assets/bfc55982-0e41-4d05-9d20-3640045e3dbe" />

<img width="1288" height="120" alt="image" src="https://github.com/user-attachments/assets/84798493-6f01-49f5-b85b-80e0f72f5d4a" />



## Sales Dashboard 
<img width="1164" height="784" alt="image" src="https://github.com/user-attachments/assets/726e2594-666a-45d7-ab2f-c395e22cc3d7" />

<p></p>


## Key Insights

**Growth is steady, but slowing:**
Net Sales ($16.9M) and Net Profit ($3.6M) are both up YoY, but growth has tapered from ~8.9% to 6.3%.

**Profitability is strong overall:**
A 21.07% profit margin (up 1.4% vs. prior year) indicates the business is becoming more profitable. 

**Profit is concentrated in Northeast cities:**
New York, Philadelphia, and Boston lead in total profit, indicating the Northeast is the primary profit engine. 

**Underperforming cities are spread across regions:**
Bottom performers (Charlotte, Phoenix, Los Angeles) are not isolated to one region, pointing to city-level execution issues rather than regional strategy alone. 

**Sales peak late in the year, but profit lags until year-end:**
Sales climb through Q4, but profit only spikes sharply in December, suggesting margin pressure during peak sales months.

**Monthly performance is inconsistent across stores:**
The heatmap shows that nearly every store struggles in January and February, with profit turning negative or flat across all locations. Performance builds through the year and peaks in Q4, indicating a heavy reliance on holiday/seasonal sales to drive annual profitability. 


## Products Dashboard 

<img width="1164" height="784" alt="image" src="https://github.com/user-attachments/assets/688fc216-6984-41d4-9011-d390ea20c6f7" />

<p></p>

## Key Insights 

**Unit growth is outpacing value growth**
Units Sold (+5.3% YoY) increased meaningfully, while Average Order Value (+0.4%) remained nearly flat. 

**Profit per order is improving, but modestly**
Average Profit per Order rose 1.8% YoY, indicating slight margin gain though not at the same pace as unit growth, suggesting the business is scaling volume faster than it is scaling value. 

**High-margin subcategories are not always top profit drivers**
Some of the highest margin categories (Phones 35.2%, Outdoor 32.2%) are strong contributors, but others with high margins (e.g. Decor 36%, Furniture 33.5%) fall into low total profit suggesting low sales volume is limiting impact. 

**Low-margin categories are dragging overall profitability**
subcategories like Accessories (15.4%) and Games (9.8%) generate weak margins and contribute to the bottom tier of profit performance, making them clear targets for pricing or cost optimization.

**Profit performance is concentrated in a few key subcategories**
Educational, Laptops, and Kitchen lead in total profit, indicating a reliance on a small group of categories to drive overall product profitiability.

**Clear gaps between high-sales and high-margin segments**
The scatterplot shows several subcategories sitting above the average margine line but left of the average sales line (high margin, low volume) representing the clearest growth opportunites. Subcategories below average profit margin but right of average sales are generating volume without proportional profitability. 

**Seasonal demand varies significantly by subcategory**
The heatmap shows Menswear and Chairs having their worst profit in January and February before recovering later in the year. Top subcategories like Educational and Laptops show steady blue throught, suggesting their profitability is less seasonal and more structually driven.

## Recommendations

**1. Strengthen performance in underperforming cities:**
Charlotte, Phoenix, and Los Angeles consistently lag in profit despite being in different regions. Recommended actions include:
  - Conduct store level audits
  - Evaluate staffing, inventory mix, and local pricing
  - Introduce targeted promotions to boost conversions

**2. Reduce margin pressure during peak sales months:**
Sales rise through Q4, but profit only spikes in December, indicating margin compression earlier in the quarter.
Recommended actions iclude:
  - Review discounting and promotional strategy in October-November
  - Optimize inventory to reduce reliance on markdowns
  - Negotiate seasonal vendor terms

**3. Address early-year performance dips:**
January and February show negative or flat profit across nearly all stores.
Recommended actions include: 
  - Launch winter-specific product bundles
  - Adjust staffing schedules to reduce labor cost during slow periods
  - Promote categories that remain stable during winter months

**4. Expand high-margin, low-volume product categories:**
Categories like Decor, Furniture, and Outdoor have strong margins but low sales volume.
Recommended actions: 
  - Increase merchandsing visibility and digital placement
  - Bundle high-margin items with popular categories
  - Test regional assortment expansion in high-performing cities

**5. Improve profitability in low-margin, high-volume categories:** 
Accessories and Games generate significant sales volume but weak margins.
Recommended actions: 
  - Reassess pricing strategy
  - Explore supplier renegotiation 


## Conclusion

This analysis provides management with a clear, data-driven roadmap to address City Market Co's flattening sales growth and operational inefficiencies. While steady overall margins and top-performing markets like the Northeast demonstrate a solid operational foundation, significant opportunities remain to optimize  underperforming store locations and align product volume with profitability. 

By executing strategic interventions, such as restructuring early-year and peak-season promotional strategies, expanind visibility for high-margin subcategories, and addressing city-level execution issues, City Market Co. can protect its margins, smooth out seasonal profit volatility, and convert revenue growth into sustained, long-term profitabilty. 









