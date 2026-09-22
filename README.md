# E-Commerce-Sales-Analysis-Business-Dashboard
An E-Commerce Sales Analysis project using a dataset obtained from Kaggle. The dataset was cleaned and validated by checking for missing values, inconsistencies, and correct data formats, while creating new variables where necessary. The cleaned data was then analyzed to generate business insights.
## Project Overview

This project presents an E-Commerce Sales Analysis conducted to transform raw sales data into meaningful business insights. The dataset was obtained from Kaggle and first evaluated for data quality, including missing values, inconsistencies, duplicate records, and data-format accuracy.

After cleaning and validating the dataset, I analyzed the data to identify sales patterns, product category performance, regional performance, payment-method trends, and revenue trends over time. The findings were then presented through an interactive Excel dashboard designed to help businesses understand their performance and support data-driven decision-making.
## Data Source & Data Wrangling

* The E-Commerce Sales dataset was obtained from Kaggle.
* The dataset contained 12 fields covering customer, order, product, sales, delivery, and payment information.
* I reviewed the dataset structure and examined the available fields.
* I checked for missing, null, and non-value entries.
* I checked for inconsistencies across the dataset.
* I validated the data types and formats of the fields, including date and currency-related fields.
* I corrected identified formatting and data-quality issues.
* I performed the initial data wrangling and cleaning to prepare the dataset for analysis.
* After cleaning the data, I identified business questions that could be answered using the dataset.
## Exploratory Data Analysis

After cleaning and validating the dataset, I conducted exploratory data analysis to understand the patterns within the data and identify areas that could provide useful business insights.

The exploration focused on the following areas:

### Sales and Product Performance

I examined revenue and quantity sold across the different product categories to understand which categories contributed most to overall sales performance.

This helped identify differences in both sales volume and revenue between categories and provided a basis for further investigation into the factors contributing to category performance.

### Regional Performance

I explored sales activity across the different regions by comparing revenue and order volumes.

This provided an overview of how sales were distributed geographically and helped identify differences in regional performance.

### Customer and Order Patterns

I examined Customer ID and Order ID to understand purchasing behavior and determine whether customers made one-time purchases or returned to make additional purchases.

This provided an initial view of customer purchasing patterns without focusing heavily on individual customers.

### Payment Methods

I analyzed the available payment methods and compared their transaction volumes and revenue contribution.

This helped identify which payment methods were most frequently used and how transaction frequency related to revenue generated.

### Delivery Performance

I also explored delivery days across regions to understand whether there were noticeable differences in delivery times between locations.

The findings from this exploratory analysis helped me identify the business questions that the dataset could answer and guided the next stage of the project.

## Business Questions

After exploring the cleaned dataset, I identified a set of business questions that could be answered using the available sales, product, regional, customer, payment, and operational data.

The questions were designed to understand overall sales performance, identify factors associated with product performance, examine regional and payment patterns, and evaluate changes in revenue and customer ratings over time.

The key business questions were:

1. **Which product category generated the highest revenue?**

2. **Which product category had the highest quantity sold?**

3. **Was the strong revenue performance of the highest-performing product category associated with pricing, discounting, or sales volume?**

4. **How did demand for the highest-performing product category differ across regions?**

5. **Which region generated the highest revenue?**

6. **How did average delivery performance compare across regions?**

7. **Which payment method was used most frequently?**

8. **Which payment method generated the highest total revenue?**

9. **How did revenue change from year to year between 2022 and 2035?**

10. **How did average customer ratings differ across product categories?**

These questions provided the direction for the detailed analysis that followed. Excel PivotTables were then used to summarize the relevant fields, compare results, identify patterns, and generate findings that could be presented through the dashboard.

## Analysis & Findings

After cleaning the E-Commerce Sales dataset and conducting exploratory analysis, I moved into the business-focused analysis stage. The objective was to answer the business questions identified during the exploration and understand patterns in sales performance, product demand, regional performance, payment behavior, customer ratings, and revenue trends.

I used **Excel PivotTables** to summarize the data, compare key measures, and identify patterns that could support business decision-making.

### 1. Which Product Category Generated the Highest Revenue?

To determine which product category contributed the most to overall revenue, I created a PivotTable using:

* **Rows:** Product Category
* **Values:** Sum of Revenue

The analysis compared the total revenue generated by Electronics, Clothing, Beauty, and Home.

**Finding:**
Electronics generated the highest total revenue among the four product categories.

Because revenue alone does not explain what contributed to this performance, I conducted additional analysis using quantity sold, average unit price, discount, and revenue per unit.

### 2. Which Product Category Had the Highest Quantity Sold?

To understand whether sales volume contributed to category revenue performance, I analyzed the total quantity sold for each product category.

| Product Category | Quantity Sold |
| ---------------- | ------------: |
| Electronics      |         7,109 |
| Clothing         |         6,171 |
| Home             |         3,949 |
| Beauty           |         2,995 |

**Finding:**
Electronics recorded the highest sales volume, with **7,109 units sold**, followed by Clothing with 6,171 units.

Electronics therefore sold **938 more units than Clothing**, the second-highest category.

This provided an important indication that sales volume was a major contributor to Electronics' high revenue.

### 3. Was the Strong Performance of Electronics Driven by Pricing or Discounting?

Since Electronics recorded the highest revenue and quantity sold, I further examined whether its performance was associated with higher prices or heavier discounting.

I compared:

* Average Unit Price
* Average Discount
* Revenue per Unit

The average unit price for Electronics was approximately **314.90**, which was higher than the other categories.

Discounts across the categories were broadly similar at around **10%**.

Revenue per unit was approximately:

| Product Category | Revenue per Unit |
| ---------------- | ---------------: |
| Electronics      |              257 |
| Beauty           |              255 |
| Clothing         |              248 |
| Home             |              248 |

**Finding:**
Electronics recorded the highest revenue per unit while also having the highest quantity sold.

Since discounts were broadly similar across categories, the analysis does not indicate that heavier discounting was the main factor behind Electronics' stronger performance.

The combination of **higher sales volume and higher revenue per unit** provides a stronger explanation for its higher total revenue in this dataset.

### 4. How Does Electronics Demand Differ Across Regions?

After identifying Electronics as the highest-revenue category, I examined how its sales volume was distributed across the four regions.

| Region | Electronics Quantity Sold |
| ------ | ------------------------: |
| East   |                     1,648 |
| North  |                     1,860 |
| South  |                     1,851 |
| West   |                     1,750 |

**Finding:**
The **North** recorded the highest absolute quantity of Electronics sold, with 1,860 units, closely followed by the South with 1,851 units.

The difference between the highest and lowest regions was **212 units**, indicating that Electronics sales were distributed across all four regions rather than being concentrated in a single region.

### 5. Which Region Generated the Highest Revenue?

I analyzed revenue across the four regions using a PivotTable with:

* **Rows:** Region
* **Values:** Sum of Revenue

This allowed me to compare the overall revenue contribution of the East, North, South, and West regions.

The regional revenue comparison was incorporated into the dashboard through the **Revenue by Region** visualization, allowing regional performance to be compared at a glance.

This analysis provides a basis for monitoring regional sales performance and identifying regions that may require further investigation.

### 6. How Does Delivery Performance Compare Across Regions?

To examine whether delivery performance differed across regions, I calculated the average delivery days for each region.

| Region | Average Delivery Days |
| ------ | --------------------: |
| East   |                  6.10 |
| North  |                  6.11 |
| South  |                  6.17 |
| West   |                  6.08 |

**Finding:**
Average delivery times were highly consistent across all four regions, with values clustered around approximately six days.

The South had the highest average delivery time at **6.17 days**, while the West had the lowest at **6.08 days**.

The difference between the highest and lowest regional averages was only **0.09 days**, or approximately two hours.

Therefore, the dataset does not show a substantial regional difference in average delivery performance.

### 7. Which Payment Method Was Used Most Frequently?

To understand payment preferences, I analyzed the number of orders associated with each payment method.

The PivotTable used:

* **Rows:** Payment Method
* **Values:** Count of Order ID

| Payment Method   | Number of Orders |
| ---------------- | ---------------: |
| Card             |            2,207 |
| Cash on Delivery |            1,774 |
| Wallet           |              956 |

**Finding:**
Card was the most frequently used payment method, followed by Cash on Delivery and Wallet.

The distribution was presented in the dashboard using a **doughnut chart**, making the relative frequency of each payment method easy to compare.

### 8. Which Payment Method Generated the Highest Revenue?

I then compared payment methods based on their total revenue.

| Payment Method   | Orders | Total Revenue |
| ---------------- | -----: | ------------: |
| Card             |  2,207 |    $2,366,248 |
| Cash on Delivery |  1,774 |    $1,788,484 |
| Wallet           |    956 |   $900,955.19 |

**Finding:**
Card generated the highest total revenue, followed by Cash on Delivery and Wallet.

Order volume and total revenue followed the same general pattern, with the payment methods having more orders also generating higher total revenue.

This indicates an association between transaction volume and total revenue in the dataset; however, it does not establish that the payment method itself caused higher revenue.

### 9. How Did Revenue Change Over Time?

To understand the overall sales trend, I analyzed revenue by year using:

* **Rows:** Order Date, grouped by Year
* **Values:** Sum of Revenue

I then created a **Yearly Revenue Trend** line chart to visualize revenue changes from **2022 through 2035**.

The yearly analysis provides a view of:

* Periods of increasing revenue
* Periods of declining revenue
* Significant fluctuations
* High-performing years
* Changes in the overall sales trend

I used yearly rather than monthly analysis because the dataset covers multiple years. A monthly comparison across all years would have made the visualization more difficult to interpret.

**Important consideration:**
The year **2035 represents a partial year in the dataset**. Therefore, its revenue should not be directly compared with the full-year figures from 2022–2034 without considering the difference in the period covered.

### 10. How Do Customer Ratings Differ by Product Category?

As a supporting analysis, I examined average customer ratings across product categories.

The PivotTable used:

* **Rows:** Product Category
* **Values:** Average of Customer Rating

| Product Category | Average Rating |
| ---------------- | -------------: |
| Beauty           |           3.01 |
| Clothing         |           3.01 |
| Electronics      |           2.95 |
| Home             |           2.94 |

**Finding:**
Average customer ratings were relatively similar across all four categories.

Beauty and Clothing recorded the highest average rating at **3.01**, while Home recorded the lowest at **2.94**.

The differences were small, so the analysis does not indicate a major variation in customer ratings between the product categories.

## Overall Findings

The analysis identified several notable patterns in the dataset.

**Electronics** was the strongest-performing product category by total revenue and quantity sold. It also recorded the highest revenue per unit. Since discounts were broadly similar across categories, the analysis suggests that its stronger performance was more closely associated with sales volume and revenue per unit than with heavier discounting.

Electronics demand was distributed across all four regions, with the **North recording the highest quantity sold**.

Payment analysis showed that **Card** was both the most frequently used payment method and the payment method associated with the highest total revenue. The same general ordering was observed for transaction volume and total revenue.

Regional delivery performance was highly consistent, with average delivery times differing by only **0.09 days** between the fastest and slowest regions.

The yearly revenue analysis provided a broader view of sales performance from **2022–2035**, while the customer-rating analysis showed relatively similar average ratings across product categories.

## Business Value

The purpose of the analysis was to transform the available sales data into information that could support business decisions.

The findings can support:

* **Product strategy:** Understanding which categories contribute most to revenue and sales volume.
* **Inventory planning:** Using sales quantity to identify categories with stronger demand.
* **Regional monitoring:** Comparing sales performance across regions.
* **Payment strategy:** Understanding payment preferences and their relationship with transaction volume and revenue.
* **Performance monitoring:** Tracking revenue patterns over time.
* **Customer experience:** Monitoring category-level customer ratings and identifying areas that may require further investigation.

## Dashboard Development

After completing the analysis, I developed an interactive **E-Commerce Sales Dashboard in Microsoft Excel** to present the key findings in a clear and accessible format.

The dashboard was built using a series of **PivotTables and PivotCharts**, which allowed the analyzed data to be summarized and presented visually.

### PivotTable Analysis

I created multiple PivotTables to support different areas of the analysis, including:

* **Regional Analysis:** Used to compare performance across regions and identify differences in regional sales.
* **Product Category Analysis:** Used to compare product categories based on revenue and quantity sold.
* **Top 10 Customers by Revenue:** Used to identify the customers who generated the highest total revenue.
* **Payment Method Analysis:** Used to compare transaction volume and revenue across payment methods.
* **Yearly Revenue Analysis:** Used to examine changes in revenue across the years covered by the dataset.
* **Delivery Analysis:** Used to compare average delivery days across regions.
* **Customer Rating Analysis:** Used to compare average customer ratings across product categories.

These PivotTables provided the underlying summaries used to create the dashboard visualizations.

### Filters and Sorting

I used Excel filtering and sorting features to make the analysis easier to navigate and interpret.

For the **Top 10 Customer** analysis, I used the Customer ID field and applied sorting and filtering to identify the customers with the highest revenue.

The data could also be arranged in **A–Z order** where appropriate, making Customer IDs and other categorical fields easier to locate and review.

### Dashboard Visualizations

The dashboard combines different visual elements to communicate the results clearly. The visualizations were selected based on the type of information being presented.

For example:

* **Charts** were used to compare categories, regions, and revenue trends.
* A **doughnut chart** was used to show the distribution of payment methods.
* **KPI cards** were used to highlight important summary metrics.
* **Slicers** were incorporated to allow users to filter and interact with the dashboard.
* A **yearly line chart** was used to show changes in revenue over time.

The use of different visualization types allowed numerical information to be converted into patterns that could be understood more quickly.

### Dashboard Design and Accessibility

I used a **blue background** and a clear visual layout to create a consistent dashboard design and make the information easy to distinguish.

The dashboard was designed with readability and simplicity in mind so that users could understand the key information without needing technical knowledge of data analysis or Excel.

Rather than presenting the results as raw tables alone, the dashboard organizes the information into visual summaries, charts, KPIs, and interactive filters. This makes it easier for users to identify important patterns and compare different aspects of the business performance.

### Interactivity

Slicers and filters allow users to interact with the dashboard and explore specific parts of the dataset.

For example, users can filter the dashboard by **Product Category** to compare the performance of different categories while the other dashboard metrics update accordingly.

This makes the dashboard more than a static report; it provides an interactive way to explore the underlying sales data and findings.
## Business Insights & Decision Support

The analysis provided several insights into the performance of the e-commerce business. These insights can help management understand where sales are coming from, identify areas of stronger demand, and monitor operational and customer-related performance.

### Product Performance

Electronics generated the highest revenue and also recorded the highest quantity sold, with **7,109 units**. It also had the highest revenue per unit among the product categories analyzed.

Since discounts were broadly similar across categories, the results suggest that the stronger performance of Electronics was more closely associated with its sales volume and revenue per unit.

**Business implication:**
The business can use this information when reviewing product demand and inventory levels, particularly for categories demonstrating stronger sales performance.

### Regional Performance

Electronics sales were distributed across all four regions, with the North recording the highest quantity sold at **1,860 units**. The relatively small difference between the regions indicates that demand was not concentrated in only one location.

Regional revenue analysis also provides a way to monitor differences in overall sales performance between locations.

**Business implication:**
Management can use regional performance data to monitor sales across locations and investigate areas where performance differs significantly.

### Payment Behavior

Card was the most frequently used payment method, with **2,207 orders**, and also generated the highest total revenue at **$2,366,248**.

Cash on Delivery followed with 1,774 orders and $1,788,484 in revenue, while Wallet recorded 956 orders and $900,955.19 in revenue.

The same general pattern between order volume and total revenue indicates an association between transaction volume and revenue in the dataset.

**Business implication:**
Understanding payment preferences can help the business monitor how customers complete transactions and ensure that commonly used payment options remain available and convenient.

### Delivery Performance

Average delivery times were very similar across all regions, ranging from **6.08 to 6.17 days**.

The small difference indicates that there was no substantial regional variation in average delivery performance within the dataset.

**Business implication:**
The business can continue monitoring delivery performance across regions and investigate larger deviations if they appear in future data.

### Revenue Trends

The yearly revenue analysis provided an overview of sales performance from **2022 to 2035**.

Tracking revenue by year allows the business to identify periods of growth, decline, or significant fluctuation and provides a basis for monitoring overall sales performance over time.

**Business implication:**
Management can use historical revenue trends as a reference when evaluating business performance and planning future sales activities, while taking into account that **2035 represents a partial year in the dataset**.

### Customer Ratings

Average customer ratings were relatively similar across all product categories, ranging from **2.94 to 3.01**.

This indicates that there was no substantial difference in average ratings between the categories within the analyzed dataset.

**Business implication:**
Category-level ratings can be monitored over time to identify changes in customer feedback and determine whether particular products or categories require further investigation.

## Decision Support

Overall, the analysis and dashboard provide a consolidated view of the business's sales performance.

The findings can support decision-making by helping management:

* Monitor high-performing product categories.
* Review inventory according to observed demand.
* Compare regional sales performance.
* Understand customer payment preferences.
* Monitor delivery performance across regions.
* Track revenue trends over time.
* Monitor customer ratings across product categories.

The dashboard therefore serves as a **decision-support tool**, allowing users to move from individual data points to a broader understanding of business performance through interactive visualizations and filters.
## Tools and Resources Used

### Microsoft Excel

Microsoft Excel was the primary tool used for the project. It was used for:

* Data cleaning and preparation
* Data wrangling
* Exploratory data analysis
* Creating PivotTables and PivotCharts
* Filtering and sorting data
* Analyzing sales, products, regions, customers, payments, and delivery performance
* Creating KPI cards
* Adding slicers and interactive filters
* Developing the final interactive dashboard
* Presenting the findings through visualizations

### Online Dashboard Icons

I sourced selected icons online and incorporated them into the Excel dashboard as visual elements.

The icons were used to represent different dashboard metrics and functions, helping improve the visual presentation and make the dashboard easier to understand and navigate.

### Tools Summary

* **Microsoft Excel:** Data cleaning, analysis, PivotTables, PivotCharts, and dashboard development
* **Online resources:** Dashboard icons and visual assets
## Project Workflow

The project followed a structured process from obtaining the dataset to developing the final dashboard and identifying business insights.

**1. Dataset Acquisition**
Obtained the E-Commerce Sales dataset from Kaggle.

**2. Data Wrangling & Cleaning**
Reviewed the dataset, checked for missing and invalid values, identified inconsistencies, validated data types and formats, and prepared the data for analysis.

**3. Exploratory Data Analysis**
Explored the cleaned dataset to understand the available variables, identify patterns, and determine the types of business questions that could be answered.

**4. Business Questions**
Developed practical business questions based on the patterns and information identified during the exploratory analysis.

**5. Analysis & Findings**
Used Excel PivotTables and PivotCharts to analyze the business questions and identify findings across products, regions, customers, payments, delivery performance, and revenue trends.

**6. Dashboard Development**
Converted the key findings into an interactive Excel dashboard using visualizations, KPI cards, slicers, filters, and dashboard design elements.

**7. Business Insights & Decision Support**
Interpreted the findings and identified how the analysis could support areas such as product planning, inventory monitoring, regional performance, payment preferences, revenue monitoring, and customer experience.

**8. Final Presentation**
Organized the analysis and dashboard into a clear portfolio project that communicates the process, findings, and potential business value.

### Workflow Summary

**Dataset Acquisition → Data Wrangling & Cleaning → EDA → Business Questions → Analysis & Findings → Dashboard Development → Business Insights & Decision Support**
## Conclusion

This project provided an opportunity to apply data analysis skills to a real-world E-Commerce Sales dataset, from data preparation and exploration to analysis, visualization, and dashboard development.

Using Microsoft Excel, I cleaned and validated the dataset, explored the available data, developed business questions, and used PivotTables and PivotCharts to identify meaningful patterns in sales, product categories, regions, payment methods, delivery performance, customer ratings, and revenue trends.

The analysis showed that Electronics was the highest-performing product category by revenue and quantity sold, while Card was the most frequently used payment method and generated the highest total revenue. The analysis also showed relatively consistent delivery performance across regions and provided an overview of revenue performance from 2022 to 2035.

The final interactive dashboard brought these findings together in a clear and accessible format, allowing users to explore the data through visualizations, KPI cards, slicers, and filters.

As my **first Excel dashboard project**, this project strengthened my practical understanding of data cleaning, exploratory analysis, PivotTable-based analysis, data visualization, dashboard development, and translating data into insights that can support business decision-making.

