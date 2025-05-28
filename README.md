#  Sales & Customer Analytics Dashboards

A business-driven Tableau project simulating a retail sales environment. Built to help sales managers, marketing teams, and executives gain insights into performance metrics, customer trends, and segmentation — using clean, interactive dashboards.

---

##  Project Description Summary

In this project, I developed two dashboards — **Sales** and **Customer** — based on a simulated retail dataset. The project mirrors real business scenarios with stakeholder-driven requirements to support data-informed decision-making.

---

##  Project Overview

-  Tools used: Tableau
-  Dashboards: Sales Overview, Customer Analysis
-  Audience: Sales managers, Marketing, Executives
-  Business goal: Enable year-over-year performance tracking, customer behavior analysis, and customer value segmentation

---

##  Executive Summary

The sales Dashboard reveals strong YoY growth in total sales (+20.4%), profit (+12.5%), and order quantity (+26.8%), driven by top-selling categories like Phones and Chairs. Notably, Copiers led in profitability, while Appliances showed the highest YoY sales growth — making it a key area for expansion. However, categories like Machines and Envelopes experienced significant sales declines, and Tables continue to operate at a loss. These trends offer actionable insights for optimizing product strategy and marketing focus.

On the Customer Dashboard, year-over-year growth in customers (+8.6%), sales per customer (+10.8%), and total orders (+28.3%) reflects a healthier and more engaged customer base. November emerged as the peak month for engagement, while January drove the highest revenue per customer. However, a significant portion of customers only place 1–3 orders, signaling retention gaps. The business should leverage seasonal trends, focus on increasing order frequency, and prioritize top-profit customers like Raymond and Tom to drive long-term value.





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

---

## 🧾 Data Description

- Sales, order, customer demographic, and product data across two years
- Cleaned in Excel and structured using SQL joins for analysis
- Segmentation logic based on total spend, recency, and order frequency

[Detailed data dictionary ➜](docs/data_description.md)

---

## 🧩 Customer Report ERD

Entity-Relationship Diagram for customer segmentation logic and data modeling.

![Customer ERD](docs/customer_report_erd.png)

---

## 📊 Dashboards Preview

### 🧾 Sales Dashboard
> View metrics like YoY sales, subcategory profit, and weekly trends.

![Sales Dashboard](images/sales_dashboard_preview.png)

### 👥 Customer Dashboard
> View KPIs, customer segment performance, and Top 10 customers by profit.

![Customer Dashboard](images/customer_dashboard_preview.png)

---

## 🚀 Dashboard Features

- 📆 Year-over-year KPI tracking
- 📈 Interactive charts with drilldowns by region, category, and time
- 🔀 Dynamic filters: year, region, category, customer segment
- 🧠 Business-friendly layout designed for managers and execs
- 🧭 Navigation between dashboards with intuitive interactivity

---

## 🔄 How to Use

1. Download the `.twbx` files from `/dashboards`
2. Open in Tableau Desktop (2022+)
3. Filter by year, category, and location to explore insights
4. Use interactive legends and charts to drill down into key trends

---

## 🧠 Learnings

- Advanced dashboard actions (highlight, filter, URL navigation)
- Designing for stakeholders (clean layout, business KPIs)
- Data storytelling through segment insights, recency & profitability

---

## 🔗 View on Tableau Public

- [🔍 View Sales Dashboard](https://public.tableau.com/profile/yourlink)
- [🔍 View Customer Dashboard](https://public.tableau.com/profile/yourlink)

---

## 🙏 Acknowledgments
This project was inspired by the teaching style and Tableau techniques shared by [Bara](https://www.youtube.com/@DataWithBaraa) on YouTube.

