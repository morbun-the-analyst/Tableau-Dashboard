#  Sales & Customer Analytics Dashboards
## Project Background


This project presents an interactive sales dashboard built in Tableau using a dataset composed of four core tables: Orders, Customers, Products, and Location. The primary goal of this analysis was to uncover insights into sales performance across different customer segmen, product subcategories, and geographic regions.

By integrating these datasets through common keys—such as Customer ID, Product ID, and Postal Code—the dashboard enables dynamic filtering and exploration of key metrics including Sales, Profit, and Quantity. Filters were provided for Customer Name, Subcategory, and detailed geographic levels including City, State, Region, and Country to support localized business decisions.

Key performance indicators (KPIs) and trends were visualized to assist stakeholders in identifying high-performing areas and products, understanding customer distribution, and recognizing opportunities for improved profitability and sales strategy refinement.




##  Project Description Summary

In this project, I developed two dashboards — **Sales** and **Customer** — based on a simulated retail dataset. The project mirrors real business scenarios with stakeholder-driven requirements to support data-informed decision-making.



##  Project Overview

-  Tools used: Tableau
-  Dashboards: Sales Overview, Customer Analysis
-  Audience: Sales managers, Marketing, Executives
-  Business goal: Enable year-over-year performance tracking, customer behavior analysis, and customer value segmentation


##  Executive Summary

The sales Dashboard reveals strong YoY growth in total sales (+20.4%), profit (+12.5%), and order quantity (+26.8%), driven by top-selling categories like Phones and Chairs. Notably, Copiers led in profitability, while Appliances showed the highest YoY sales growth — making it a key area for expansion. However, categories like Machines and Envelopes experienced significant sales declines, and Tables continue to operate at a loss. These trends offer actionable insights for optimizing product strategy and marketing focus.

On the Customer Dashboard, year-over-year growth in customers (+8.6%), sales per customer (+10.8%), and total orders (+28.3%) reflects a healthier and more engaged customer base. November emerged as the peak month for engagement, while January drove the highest revenue per customer. However, a significant portion of customers only place 1–3 orders, signaling retention gaps. The business should leverage seasonal trends, focus on increasing order frequency, and prioritize top-profit customers like Raymond and Tom to drive long-term value.

## Data Description

- **Overview**
This dataset contains four relational tables: `Orders`, `Customers`, `Products`, and `Location`. These tables support a Tableau sales dashboard focused on tracking key performance indicators (KPIs) such as profit, sales, and quantity sold, with the ability to filter by customer and geographic location.



### 📦 Table: Orders

| Field Name       | Description                                | Type    |
|------------------|---------------------------------------------|---------|
| `OrderID (PK)`   | Unique identifier for each order            | Integer |
| `OrderDate`      | Date the order was placed                   | Date    |
| `Profit`         | Profit made on the order                    | Float   |
| `Quantity`       | Number of items ordered                     | Integer |
| `Sales`          | Total value of the order                    | Float   |
| `CustomerID (FK)`| Foreign key referencing `Customers` table   | String  |
| `ProductID (FK)` | Foreign key referencing `Products` table    | String  |
| `PostalCode (FK)`| Foreign key referencing `Location` table    | String  |

### 👥 Table: Customers

| Field Name        | Description                     | Type   |
|-------------------|----------------------------------|--------|
| `CustomerID (PK)` | Unique identifier for customer   | String |
| `CustomerName`    | Full name of the customer        | String |

### 🛒 Table: Products

| Field Name        | Description                       | Type   |
|-------------------|------------------------------------|--------|
| `ProductID (PK)`  | Unique product identifier          | String |
| `SubCategory`     | Product sub-category (e.g., Chairs, Phones) | String |

### 🌍 Table: Location

| Field Name         | Description              | Type   |
|--------------------|---------------------------|--------|
| `PostalCode (PK)`  | Unique postal code        | String |
| `Country`          | Country name              | String |
| `Region`           | Region within the country | String |
| `State`            | State or province         | String |
| `City`             | City                      | String |


### 🔗 Relationships

- `Orders.CustomerID` → `Customers.CustomerID`
- `Orders.ProductID` → `Products.ProductID`
- `Orders.PostalCode` → `Location.PostalCode`

---

- **NB** All foreign key relationships are one-to-many, originating from the `Orders` table which acts as the transactional fact table in this sales dataset.


## Dashboard  ERD
<img src="https://github.com/morbun-the-analyst/Tableau-Dashboard/blob/main/visualization/Screenshot%202025-05-29%20133428.png?raw=true" alt="Screenshot 2025-05-29 133428" width="300"/>



## Sales Dashboard Insights  
 -**Overall Growth in Sales Metrics**

-Total sales ↑ 20.4%, profit ↑ 12.5%, and quantity ↑ 26.8% YoY
-Indicates strong customer engagement. 

-**High Performers**

-Phones, Chairs, and Binders drove the highest sales this year
-Appliances had the highest YoY growth, suggesting an emerging category

-**Top Profit Driver**

-Copiers generated the highest profit of 63k  and ranked among the top 5 in sales — indicating high-margin performance

-**Underperformers**

-Machines, Envelopes, and Tables all showed YoY sales decline
-Machines: -22.1%, Envelopes: -28%, Tables: barely grew (+0.1%)
-Tables showed the highest loss despite a minor improvement in sales

## Customer Dashboard Insights 

-**Customer Growth & Engagement**

-Total customers ↑ 8.6%, sales per customer ↑ 10.8%, and total orders ↑ 28.3% YoY
-Indicates stronger customer base and more frequent purchasing behavior

-**Monthly Customer Behavior**

-November: highest number of customers and total orders (likely seasonal peak)
-February: lowest customer activity — potential dip due to post-holiday lull
-January: highest sales per customer — early-year big spenders
-April: lowest sales per customer — possible disengagement or smaller-ticket items

-**Order Distribution**

-Majority of customers placed 1–3 orders
-200 (1 order), 200 (2 orders), and 156 (3 orders)
-Suggests a large base of low-frequency buyers — opportunity to improve retention or upselling

-**Top Customers by Profit**

-Highest contributors: Raymond, Tom, and one other (4.5K)
-These VIP customers offer strong ROI and should be prioritized for  eloyalty effortse summary ➜](docs/executive_summary.md)



##  Dashboards Preview

### Sales Dashboard
> View metrics like YoY sales, subcategory profit, and weekly trends.

![Sales Dashboard](images/sales_dashboard_preview.png)

### Customer Dashboard
> View KPIs, customer segment performance, and Top 10 customers by profit.

![Customer Dashboard](images/customer_dashboard_preview.png)

---

##  Dashboard Features

-  Year-over-year KPI tracking
- Interactive charts with drilldowns by region, category, and time
- Dynamic filters: year, region, category, customer segment
- Business-friendly layout designed for managers and execs
- Navigation between dashboards with intuitive interactivity


##  Learnings

- Advanced dashboard actions (highlight, filter, URL navigation)
- Designing for stakeholders (clean layout, business KPIs)
- Data storytelling through segment insights, recency & profitability


## Recommendations
-**Focus on Retention and Frequency**
- Most customers place only 1–3 orders → introduce loyalty programs or incentives for repeat purchases
-	Capitalize on January & November Peaks
- January: high AOV per customer — ideal time for product launches or upsells
-	November: top engagement — double down on promotions, flash sales, and remarketing
- **Target Low-Activity Months**
-	Develop campaigns or re-engagement offers for April and February, where both engagement and revenue dip
-**Nurture Top Customers**
-	Profile and replicate behaviors of top customers like Raymond and Tom
-	Consider personal outreach or VIP experiences to retain and expand their lifetime

## Clarifying questions $ Caveats

## 🙏 Acknowledgments
This project was inspired by the teaching style and Tableau techniques shared by [Bara](https://www.youtube.com/@DataWithBaraa) on YouTube.

