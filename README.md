👨🏻‍💻Customer Behavior Data Analyst Portfolio Project:
This project represents a complete, industry standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

The goal of this project is to simulate a corporate-grade end-to-end data analytics workflow, demonstrating the ability to translate raw data into strategic business intelligence by:



📊 **Step 1: Dataset Understanding**

**Dataset details:**

* **Rows:** 3,900
* **Columns:** 18
* **Includes:**

  * Demographics (Age, Gender, Location, Subscription Status)
  * Purchase info (Item, Category, Purchase Amount, Season, Size, Color)
  * Shopping behavior (Discount, Promo Code, Frequency, Rating, Shipping Type)
 **Missing data:** 37 missing values in *Review Rating*
This step gives an overview of data quality and completeness before analysis.


🧹 **Step 2: Data Cleaning & Exploration (Python)**
**Process:**

1. **Load Data:** Imported using `pandas`.
2. **Explore Data:** Used `.info()` and `.describe()` to understand structure and stats.
3. **Handle Missing Values:** Filled missing review ratings using the **median** rating of each product category.
4. **Standardize Columns:** Renamed all column names to `snake_case` format for clarity.
5. **Feature Engineering:**
   * Created **`age_group`** by binning customer ages.
   * Created **`purchase_frequency_days`** from timestamps.
6. **Check Data Consistency:**

   * Verified if `discount_applied` and `promo_code_used` were redundant → dropped `promo_code_used`.
7. **Database Integration:** Loaded the cleaned dataset into **PostgreSQL** for SQL-based analysis.



🧠 **Step 3: Data Analysis using SQL**
**Goal:** Answer key business questions with structured queries in PostgreSQL.

**Insights Extracted:**
1. **Revenue by Gender** – Compared spending by male vs. female customers.
2. **High-Spending Discount Users** – Found customers who used discounts but spent above average.
3. **Top 5 Products by Rating** – Identified products with best review scores.
4. **Shipping Type Comparison** – Compared spending between Standard and Express shipping.
5. **Subscribers vs. Non-Subscribers** – Compared their average spend and total revenue.
6. **Discount-Dependent Products** – Found products most frequently bought with discounts.
7. **Customer Segmentation** – Categorized customers into *New*, *Returning*, *Loyal*.
8. **Top 3 Products per Category** – Highlighted most purchased items by category.
9. **Repeat Buyers & Subscriptions** – Checked if repeat buyers tend to subscribe.
10. **Revenue by Age Group** – Analyzed which age groups contribute most to revenue.


 📈 **Step 4: Dashboard Creation (Power BI)**
* Built an **interactive dashboard** to visualize insights.
* Included KPIs like revenue, top products, and customer segments.
* Helped communicate findings clearly to stakeholders.


 💡 **Step 5: Business Recommendations**
Based on analysis and insights:
* Boost Subscriptions: Offer exclusive benefits to encourage more sign-ups.
* Loyalty Programs: Reward repeat buyers to increase retention.
* Review Discount Policy: Ensure discounts drive sales without reducing margins.
* Product Positioning: Promote top-rated and popular products.
* Targeted Marketing: Focus on profitable age groups and express-shipping customers.








