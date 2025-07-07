# OSCAR-CHOCOLATE-SALES-ANALYSIS
The Oscar Chocolate Sales Analysis has successfully revealed vital trends, revenue drivers, and performance benchmarks for HILDA PLUS. 
![Screenshot 2025-05-27 165139](https://github.com/user-attachments/assets/a06b2243-c579-4cd5-9f6c-afd08d6f7dd8)
Introduction
The Oscar Chocolate Sales Analysis project is a data-driven initiative aimed at evaluating the performance of various chocolate products, sales personnel, and markets across different countries. Utilizing interactive visualizations and dynamic filters, the dashboard delivers a holistic view of revenue generation, sales trends, product demand, and geographical performance. The analysis supports the strategic decision-making of HILDA PLUS, the company behind the Oscar Chocolate brand.

2. Purpose of the Project

The primary purpose of the Oscar Chocolate Sales Analysis is to:

Monitor sales performance over time.
Identify the top-performing salespersons and products.
Evaluate geographical markets to determine strong and weak regions.
Understand customer buying behavior based on order quantities and day preferences.
Optimize inventory and shipping based on revenue contribution.
Support strategic marketing, distribution, and sales planning decisions with data.
3. Objectives of the Project

The key objectives include:

Determining the top-performing salesperson, product, and country by revenue.
Analyzing monthly revenue trends to identify peak and off-peak periods.
Evaluating order quantity distribution by day to optimize operational workflow.
Understanding product demand patterns through visual product segmentation.
Quantifying the sales contribution by each country and recommending market focus.
Benchmarking sales performance among staff members to identify training or incentive needs.
4. Problem Being Addressed

The project addresses several business challenges:

Inconsistent sales performance across time and personnel, requiring analysis to identify root causes.
Unclear product popularity trends, making inventory and marketing strategies inefficient.
Geographical disparity in revenue contribution, necessitating localized strategy development.
Lack of real-time, data-informed decisions due to scattered and raw data.
Inefficient resource allocation due to the absence of consolidated performance metrics.
2. Key Dataset Used

The analysis was conducted using structured sales data sourced from Kaggle.com. Though coined HILDA PLUS as the company operating in Oscar chocolate. Key datasets include:

Sales Transactions Data: Date, product name, quantity sold, revenue amount.
Salesperson Performance Data: Sales volume and revenue per individual.
Product Inventory Data: SKUs, product names, and categories.
Geographic Data: Sales segmented by countries such as Australia, UK, India, USA, Canada, and New Zealand.
Shipping & Logistics Data: Number of boxes shipped and revenue generated per box.
2.2. Methodology

The methodology for this project includes:

Data Extraction and Cleaning: Raw sales data was gathered from Kaggle.com under HILDA PLUS databases and cleaned to remove inconsistencies and duplicates.
Data Modeling and Integration: Sales, product, personnel, and geography datasets were linked through relational modeling in Power BI.
Dashboard Development:
- Visual tools such as bar charts, pie charts, line graphs, and treemaps were used.

- Interactive filters were implemented for Date, Day Name, Salesperson, and Country to allow flexible user interaction.

Key Metrics Computation:
- Total Revenue: ₦6,183,625.

- Top Salesperson: Ches Bonnell.

- Top Product: Smooth Silky Salty.

- Top Country by Revenue: Australia (₦1.14M).

- Most Sold Products: 50% Dark Bites, Smooth Silky Salty, Caramel Stuffed Bars, Spicy Special Slims, Eclairs.

Time Series Analysis: Revenue trend was analyzed monthly, revealing highest performance in June (₦0.87M) and July (₦0.80M).
Customer Behavior Insight: Day-of-order distribution showed Monday as the highest with 41K orders, followed by other weekdays.
Sales Contribution Analysis: Treemaps and pie charts showed which products and shipping patterns drove the most revenue.
3.0 STORY OF THE DATA

3.1. Data Source

The data used in this analysis originates from Kaggle.com but coined to HILDA PLUS, the retail management system behind Oscar Chocolate’s sales and distribution operations. The system captures daily transaction logs, product inventory records, and sales personnel activity across multiple countries. Data was extracted from the internal enterprise resource planning (ERP) and point-of-sale (POS) systems.

3.2. Data Collection Process

Sales Transactions were automatically logged at each point-of-sale terminal and synced to a centralized cloud-based system daily.
Product Information was pulled from the inventory and product master database.
Personnel Activity was monitored through user IDs tied to each sales transaction.
Geographical Tags were assigned based on billing/shipping addresses or retail outlet location.
Order Metadata (day of week, order quantity, and revenue) was derived using timestamps and transaction IDs.
All data was exported in structured formats (CSV and Excel) and loaded into Power BI for modeling and visualization.

3.3. Data Structure

The data model was built on several interlinked tables. Key components include:

Sales Table: Includes Date, OrderID, Product, Quantity, Amount, Salesperson, and Country.
Product Table: Contains Product Name, Product Category, Unit Price, SKU.
Employee Table: Maps Salesperson ID to Salesperson Name.
Shipping Table: Includes Boxes Shipped, Shipping Cost, Revenue per Box.
Calendar Table: Derives Day Name, Month, and Year from order dates for time-based analysis.
Relationships were modeled in a star schema with the sales fact table at the center, enabling fast and flexible querying.

4 DATA SPLITTING AND PREPROCESSING

4.1. Purpose

The purpose of data preprocessing and splitting is to ensure that the dataset used in analysis is accurate, consistent, and ready for decision-making. Preprocessing enhances data quality by removing errors and structuring it for visualization. Splitting the data helps in analyzing performance across different dimensions such as time, geography, product, and personnel, enabling targeted insights.

4.2. Data Cleaning

The raw dataset was subjected to cleaning processes, which included:

Removal of duplicates to ensure accurate performance measurement.
Standardization of date formats to enable proper time-series analysis.
Correction of inconsistent entries (e.g., country names like “U.S.A.” and “USA” were unified).
Trimming whitespace and formatting in categorical variables (e.g., product names and sales personnel).
4.3. Handling Missing Values

Missing or incomplete data was handled using the following strategies:

Null entries in revenue or product fields were flagged and excluded from critical KPI computations.
Missing shipping box data was estimated using average box-per-sale metrics or excluded if insufficient context existed.
Where values like Day Name were not provided, they were reconstructed from transaction dates using a calendar table.
4.4. Data Transformation

Transformation operations included:

Aggregation of daily transactions into monthly revenue.
Normalization of numerical data to facilitate accurate visual comparisons.
Deriving fields such as:
Day Name from transaction Date
Revenue per Box
Order Volume per Day
Salesperson Ranking
5. Data Splitting

To enable meaningful business insights, the data was split across the following dimensions:

Time-Based: Monthly and daily analysis (January–August)
Geographical: By country (e.g., Australia, UK, India)
Product-Based: By product type and name
Personnel-Based: By individual salesperson performance
Order Metrics: Revenue, quantity, number of boxes shipped
This dimensional splitting allows the dashboard to support dynamic filtering and drill-down analysis in Power BI.

6. Industry Context

The chocolate and confectionery industry is highly consumer-driven, with seasonal trends, strong brand loyalty, and product-specific preferences. Sales data analysis helps:

Forecast demand based on historical patterns.
Optimize product mix by identifying high-performers.
Streamline logistics by understanding shipping vs. sales value.
Enhance marketing efforts based on customer ordering behavior.
7. Stakeholders

The key stakeholders benefiting from this data processing and analysis include:

Sales Managers — to evaluate staff performance and set sales targets.
Marketing Teams — to identify bestsellers and target promotions effectively.
Inventory Managers — to plan procurement based on product trends.
Executive Leadership — for strategic decision-making and resource allocation.
Country/Regional Managers — to assess market-specific opportunities and challenges.
8. Value to the Industry

Through this preprocessing and structured analysis:

The sales strategy becomes data-informed rather than intuition-based.
Marketing campaigns can be aligned with high-performing days and products.
Inventory waste can be reduced by aligning supply with demand patterns.
It enables market prioritization, directing investment to top-performing regions.
Provides a framework for performance benchmarking and continuous improvement.
5. PRE-ANALYSIS

5.1. Key Trends Identified

From the early exploration of the dataset, the following key trends were identified:

Strong Monthly Revenue Growth: Revenue shows a consistent rise from January, peaking in June (₦0.87M) and maintaining high performance in July (₦0.80M). This suggests mid-year sales spikes, possibly due to campaigns or seasonal demand.
Top Performing Salesperson: Ches Bonnell leads with ₦320.9K in revenue, with other staff also performing strongly. This points to a competitive sales team with room for performance incentives.
Best-Selling Product: Smooth Silky Salty is the top-grossing product, frequently appearing in top rankings, followed by 50% Dark Bites and Caramel Stuffed Bars.
Highest Revenue by Country: Australia stands out as the most lucrative market (₦1.14M), followed closely by the UK and India.
Order Pattern by Day: Mondays see the highest number of orders (41K), showing a strong start-of-week buying behavior.
Box Shipment Revenue Contribution: Only 3% of revenue is associated with the number of boxes shipped, while 97% ties directly to sales — highlighting product over volume logistics.
2. Potential Correlations Identified

Several potential relationships and correlations emerged during pre-analysis:

Sales vs. Day of the Week: High sales are correlated with Mondays, suggesting a behavioral pattern or the effect of weekend promotions.
Product Popularity vs. Revenue: Products with higher sales quantity (e.g., Smooth Silky Salty) also tend to drive more revenue, hinting at a direct correlation between volume and profitability for certain SKUs.
Geography vs. Revenue: Countries with the highest transaction volumes also report the highest revenue, suggesting population or brand preference might be influencing results.
Month vs. Revenue: Revenue climbs as the year progresses, possibly aligning with seasonal demand, implying a positive correlation between time and sales performance.
3. Initial Insights

Sales Efforts are Consistent: Sales are well distributed among the team, indicating strong collaboration and balanced performance.
Strong Product Portfolio: Multiple products are performing well, suggesting a diverse and well-received product lineup.
Monday Strategy: With Mondays showing the most customer activity, launching promotions or campaigns on weekends could boost sales performance even more.
Australia as a Growth Hub: Australia’s dominance in revenue indicates a potential flagship market for brand expansion and investment.
Revenue Not Dependent on Box Volume: Since 97% of revenue isn’t tied to shipping volume, logistics optimizations could yield cost savings without harming revenue streams.
6 IN-ANALYSIS

6.1. Ongoing Observations and Unconfirmed Insights

As the analysis progressed, several trends and patterns emerged that appeared insightful but require deeper validation before being considered conclusive:

Monthly Revenue Fluctuations:
- While revenue generally increases from January to June, there are slight dips in March and August, suggesting possible external factors like supply constraints or market disruptions. These variations require further exploration using marketing and operations data.

Product Dominance:
- Although products like Smooth Silky Salty and 50% Dark Bites dominate, some lesser-known products may be growing in popularity, which might not yet reflect significantly in revenue but could become emerging leaders.

Salesperson Performance Consistency:
- While Ches Bonnell is top overall, it’s unclear whether his dominance is consistent month-by-month or skewed by high performance in just a few months. Temporal breakdowns per staff would help confirm this insight.

Geographic Growth Patterns:
- Australia leads in revenue, but trends over time are not clearly visible per country. It’s unclear whether Australia’s lead is stable or declining relative to other countries.

Order Day Anomaly:
- Monday consistently records the highest order count, but Tuesday to Sunday show no clear decreasing or increasing pattern. Further behavioral research or customer segmentation might explain this irregularity.

7. POST-ANALYSIS AND INSIGHTS

7.1. Key Findings (Confirmed Through Full Analysis)

After completing the full data analysis using the interactive Power BI dashboard, the following key findings were confirmed with confidence:

Top Salesperson: Ches Bonnell leads in total revenue (₦320.9K), closely followed by other sales personnel, confirming consistent top-tier performance.
Top Product: Smooth Silky Salty emerged as the most revenue-generating product, maintaining dominance across different months and customer order volumes.
Best Revenue Month: June recorded the highest monthly revenue (₦0.87M), followed by July, confirming mid-year as the peak sales period.
Highest Sales Country: Australia contributes the most revenue (₦1.14M), affirming its position as the brand’s strongest international market.
Order Volume Peak: Monday remains the top day for orders (41K), with consistent engagement throughout the week, confirming earlier behavior-based assumptions.
Balanced Product Performance: Aside from top products, others such as Caramel Stuffed Bars, Eclairs, and Spicy Slims also maintain steady performance, supporting a well-diversified product base.
3. Insights Beyond Initial Expectations

The dataset analysis also revealed several unexpected or deeper insights not evident in earlier phases:

Revenue Disproportionate to Shipment Volume: Despite a large number of products sold, only 3% of revenue is tied to the number of boxes shipped. This suggests that high-value orders are compact, and logistics costs could be optimized without impacting revenue.
Consistent Salesperson Contribution: No single individual overly dominates the sales pipeline. The top five salespeople share performance fairly equally — pointing to a well-balanced and replicable sales process.
Underexploited Markets: India and New Zealand show promising revenue figures but are not yet at their full potential compared to Australia and the UK. Targeted expansion in these countries could yield growth.
Sales vs. Day Behavior Stability: Contrary to assumptions that sales taper off after Monday, order volume remains surprisingly stable from Tuesday to Friday, indicating sustained engagement throughout the workweek.
Potential for Inventory Optimization: Multiple products with similar sales volumes suggest opportunity for SKU rationalization or bundling strategies to streamline stock while maximizing shelf impact.
8. OBSERVATIONS AND RECOMMENDATIONS

8.1 OBSERVATIONS

Top Performer: Ches Bonnell is the top-performing salesperson with ₦320.9K in sales, marginally ahead of others suggesting a highly competitive sales team.
Top Product: Smooth Silky Salty emerged as the most popular and high-revenue-generating product, featuring prominently both in sales amount and volume.
Best Month for Revenue: June (₦0.87M) recorded the highest monthly revenue, indicating seasonal trends or successful campaigns.
Geographical Insights: Australia leads in revenue (₦1.14M), followed closely by the UK and India. These three markets represent significant growth opportunities.
Order Behavior: Most orders were placed on Monday (41K orders), implying the start of the week is crucial for customer engagement.
Product Sales Distribution: Products like 50% Dark Bites, Smooth Silky Salty, and Caramel Stuffed Bars dominate sales, each with 9K–10K units sold.
Shipping Pattern: Only 3% of the revenue comes from the number of boxes shipped, while 97% is tied directly to amount sold, showing bulk orders may be consolidated in fewer shipments.
8.2. Insights & Interpretation

Sales are relatively stable from February to May but peak in June, suggesting targeted marketing or seasonality may influence buyer behavior.
There is no single dominant salesperson, pointing to a well-distributed performance culture — an opportunity to invest in broad training rather than selective promotion.
Most products have uniform sales, with only slight variation, suggesting balanced inventory planning is crucial to avoid overstocking or stockouts.
High sales on Mondays could imply successful weekend promotions or customer restocking behavior at the week’s start.
8.3. Recommendations

Market Expansion: Increase marketing investment in Australia, UK, and India, as they are leading in revenue generation.
Promotional Timing: Launch new promotions and products on or before Mondays to capitalize on high customer order activity.
Sales Incentives: Introduce bonus schemes to encourage competition among top salespeople to further boost motivation and results.
Focus on Bestsellers: Boost production and inventory of Smooth Silky Salty and 50% Dark Bites due to their consistent high demand.
Refine Shipping Strategy: Investigate box utilization efficiency and optimize logistics to reduce costs or increase throughput where possible.
9.0. Conclusion

The Oscar Chocolate Sales Analysis has successfully revealed vital trends, revenue drivers, and performance benchmarks for HILDA PLUS. With total revenue reaching ₦6.18M, and top salespersons and countries identified, the company is well-positioned to make data-backed decisions. The findings underscore the importance of product-specific focus, regional strategies, and leveraging order behavior patterns for future growth.

10. Future Research Directions

Incorporate customer demographic data to analyze purchasing behavior.
Include profitability metrics, not just revenue, for better margin-based decision-making.
Introduce seasonality analysis with multi-year data for more accurate forecasting.
Evaluate the impact of promotions/marketing campaigns on revenue spikes.
11. References

Internal Sales Data (HILDA PLUS) cum kaggle.com
Dashboard Visualization from Power BI
Data analysis performed on Excel and Power BI
Appendix: Dataset Dimensions

Sales by Date
Salesperson Details
Product Type and Category
Country of Sale
Revenue and Quantity Sold
Shipping Box Count
