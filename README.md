# Customer Shopping Behavior: End-to-End Data Analytics

## 📌 Overview

This project provides a comprehensive analysis of customer purchasing patterns for a retail dataset. By leveraging **Python** for data engineering, **SQL** for deep-dive querying, and **Power BI** for visualization, the project identifies key drivers of revenue, the impact of subscription programs, and customer segmentation strategies.

**Business Goal:** To identify high-value customer segments and analyze the correlation between subscription status and spending behavior to optimize marketing ROI.

---

## 📂 Dataset

* **Source:** Customer Shopping Behavior Dataset (3,900 records).
* **Key Features:** Customer ID, Age, Gender, Purchase Amount (USD), Category, Subscription Status, Shipping Type, and Previous Purchases.
* **Target Metrics:** Revenue, Review Ratings, and Purchase Frequency.

---

## 🛠️ Tech Stack

* **Data Processing:** Python (Pandas, NumPy)
* **Database:** SQL Server / MySQL
* **Visualization:** Power BI
* **Presentation:** Gamma AI (Presentation) & Microsoft Word (Reporting)

---

## 🚀 Project Steps

### 1. Data Cleaning & Feature Engineering (Python)

Using Jupyter Notebook, I transformed the raw CSV into a structured format ready for analysis:

* **Handling Missing Values:** Imputed missing `Review Ratings` using the median value per category to maintain data distribution.
* **Feature Engineering:** * Created `age_group` (e.g., 18-30, 31-45, etc.) to analyze demographic trends.
* Derived `purchase_frequency_days` to quantify customer loyalty.


* **Data Refinement:** Dropped redundant features like `promo_code_used` to simplify the model.

### 2. Advanced SQL Analysis

The cleaned data was migrated to a relational database where I executed complex queries to extract business logic:

* **Customer Segmentation:** Used **CTEs** to categorize customers into *New*, *Returning*, and *Loyal* based on purchase history.
* **Ranking & Window Functions:** Employed `ROW_NUMBER()` and `PARTITION BY` to identify the top 3 most purchased products within every category.
* **Revenue Deep-Dive:** Compared average spend between Subscribed vs. Non-Subscribed users and analyzed shipping method preferences.

### 3. Power BI Dashboard

Developed an interactive dashboard to translate raw numbers into visual stories:

* **Sales Overview:** Tracking Total Revenue, Avg. Purchase Value, and Avg. Rating.
* **Demographic Insights:** Breakdown of spending by Gender and Age Group.
* **Behavioral Analysis:** A comparison of Subscription Status vs. Revenue contribution.
* **Geographic Mapping:** Sales distribution across different locations.

### 4. Strategic Reporting

* **Gamma AI Presentation:** Created a stakeholder-ready slide deck summarizing the "So-What" of the data.
* **Final Report:** Documented methodology, data limitations, and actionable business recommendations.

---

## 📈 Key Results & Insights

* **Subscription Impact:** Subscribed customers contribute significantly higher lifetime value despite representing a smaller portion of the total base.
* **Product Performance:** The **Clothing** category dominates in volume, while specific items in **Accessories** hold the highest average review ratings ($4.0+$).
* **Loyalty Trends:** "Loyal" customers (15+ previous purchases) are $25\%$ more likely to choose Express Shipping.
* **Gender Spend:** Male vs. Female revenue distribution shows [Insert specific finding from your SQL Query 1 here].

---

## ⚙️ How to Run

1. **Prerequisites:** Install Python 3.x and Power BI Desktop.
2. **Data Setup:** * Run the Jupyter Notebook `Customer_Shopping_Behavior_Analysis.ipynb` to generate the cleaned data.
* Import the CSV into your SQL Environment.


3. **SQL Queries:** Execute the scripts in `customer_behavior_sql_queries.sql` to view the calculated KPIs.
4. **Dashboard:** Open the `.pbix` file to explore the interactive visualizations.

---

## 📬 Contact

**[Anaswara E]** [(https://www.linkedin.com/in/anaswara-e)] | [anaswaraeshaji@gmail.com]

---

### **Quick Tips for your GitHub:**

1. **Clear the Output:** Before uploading your `.ipynb` file, go to *Cell > All Output > Clear* so the file loads quickly on GitHub.
2. **Add a Screenshot:** Place a `.png` of your Power BI dashboard in a folder named `images` and link it in the "Dashboard" section of this README.
3. **Requirements File:** Include a `requirements.txt` with `pandas` and `numpy` listed.
