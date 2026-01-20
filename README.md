#  Business Sales Performance Analytics of an Online Retail Store

##  Project Overview

This project analyzes historical transactional data from an online retail store to evaluate overall sales performance and uncover actionable business insights. The analysis focuses on revenue trends, product performance, geographic contribution, and key business KPIs to support data-driven decision-making.

The project demonstrates an end-to-end analytics workflow, from data cleaning and feature engineering to exploratory analysis and dashboard-ready outputs.

---

##  Business Problem

The business has access to large volumes of transactional sales data but lacks a clear, consolidated view of performance across:

* Time (monthly and quarterly trends)
* Products
* Geographic markets
* Core sales KPIs

Without structured analysis, decision-makers have limited visibility into revenue drivers, underperforming areas, and growth opportunities.

---

##  Project Objectives

* Assess overall sales performance using revenue, order volume, and trends over time
* Identify top-performing and underperforming products by revenue contribution
* Analyze regional sales performance to understand market concentration
* Evaluate key KPIs such as:

  * Total Revenue
  * Total Orders
  * Average Order Value (AOV)
* Generate insights and recommendations that can inform sales and growth strategy

---

##  Key Business Questions

* How has revenue changed over time?
* Which products contribute the most to total revenue?
* Which countries generate the highest sales?
* Are there identifiable underperforming or high-growth segments?
* What factors are driving overall business performance?

---

##  Dataset Overview

* **Source:** Online Retail transactional dataset
* **Records:** 541,909 rows
* **Features:** 8 columns

### Key Fields

* `InvoiceNo` – Transaction identifier
* `InvoiceDate` – Date of purchase
* `Quantity` – Number of items purchased
* `UnitPrice` – Price per item
* `CustomerID` – Customer identifier
* `Country` – Customer location

---

##  Data Cleaning & Preparation

The dataset was cleaned and transformed to ensure accuracy and usability:

* Converted `InvoiceDate` to datetime format
* Handled mixed date formats and whitespace issues
* Removed records with missing product descriptions
* Replaced missing `CustomerID` values with `"Unknown"`
* Ensured numeric integrity for Quantity and UnitPrice
* Created a **Revenue** feature (`Quantity × UnitPrice`)
* Separated **cancelled orders** from completed sales for accurate revenue analysis

---

##  Feature Engineering

Additional time-based features were created to support trend analysis:

* `Month`
* `Year`
* `Quarter`

These features enabled monthly, quarterly, and seasonal performance analysis.

---

##  Key Performance Indicators (KPIs)

* **Total Revenue:** 10.64M
* **Total Orders:** 20,610
* **Average Order Value (AOV):** 516.48
* **Revenue Lost from Cancelled Orders:** −896,812

>  The dataset does not include cost data. Profitability is estimated using an assumed average gross margin (30%) for comparative and trend analysis only.

---

##  Exploratory Data Analysis (EDA)

### Revenue Trends

* Revenue exhibits clear **seasonality**
* Lower performance in early months of the year
* Strong growth observed from September to November
* November records the highest revenue
* Final month decline is likely due to incomplete data

### Product Performance

* Revenue is highly concentrated among a small number of products
* A small set of products generates a disproportionately large share of revenue
* Indicates dependency risk on top-performing products

### Regional Analysis

* The United Kingdom dominates overall revenue
* International markets contribute relatively small shares
* Highlights opportunities for geographic diversification

### Order Value Distribution

* Order values are heavily right-skewed
* Majority of orders are low-value
* A small number of high-value orders contribute significantly to total revenue

---

##  Tableau Dashboard

A clean, analysis-ready dataset was exported for visualization in Tableau.

**Dashboard features include:**

* KPI summary (Revenue, Orders, AOV)
* Monthly revenue trend analysis
* Top products by revenue
* Revenue by country
* Interactive filters for time and geography

---

##  Key Conclusions

* Sales performance shows strong seasonal patterns
* Revenue is concentrated in a limited number of products and one primary market
* High-value orders play a significant role in overall revenue
* Cancelled orders represent a measurable revenue loss

---

##  Business Recommendations

* Investigate seasonality and promotional strategies driving revenue peaks
* Reduce reliance on top products by promoting mid-performing items
* Expand and optimize international market strategy to reduce geographic risk
* Segment customers based on order value to enable targeted pricing and promotions
* Analyze cancellation drivers to reduce revenue leakage

---

##  Tools & Technologies

* **Python:** Pandas, NumPy, Matplotlib, Seaborn
* **Visualization:** Tableau
* **Environment:** Google Colab
* **Version Control:** Git & GitHub

---

##  Project Outputs

* Cleaned, dashboard-ready dataset
* Exploratory analysis notebook
* Interactive Tableau dashboard
* Business insights and actionable recommendations

---



