# 📦 Amazon Sales & Logistics Performance Analysis

## 🚨 The Business Problem
Massive revenue (€1.10 Billion) doesn't automatically equal high profitability. Management raised concerns about skyrocketing logistics costs eating into the margins. The goal of this project (analyzing a dataset of 100,000 orders) is to identify hidden cost traps within the shipping process and provide data-driven, actionable solutions for the management team.

## 🎥 Dashboard Preview & Interactivity
<img width="1743" height="928" alt="image" src="https://github.com/user-attachments/assets/17c7c34c-ac68-4579-a5f6-7bcdbe7100a8" />


## 💡 Key Insights & Results
By modeling the data and isolating specific KPIs using DAX, the following critical business insights were uncovered:

1. **The Return Cost Black Hole:** Although the overall cancellation and return rate (Cancelled/Returned) is remarkably low at just ~5%, this tiny fraction is responsible for nearly **€45,000 in "dead" shipping costs** (`ShippingCost`).
2. **The US Factor:** Out of this €45,000 loss, a staggering **€32,000 (over 70%) originates solely from the United States**.
3. **Category Independence:** The issue rate remains constant at around 6% across almost all product categories (Home & Kitchen, Books, Clothing, Electronics). 

**Conclusion & Actionable Recommendation:**
Since the issue is spread evenly across all categories, this is not a product problem (e.g., poorly fitting clothing), but a **structural logistics problem**. I strongly recommend an immediate audit of the US logistics network (evaluating the geographical distances between fulfillment centers and customers, as well as renegotiating carrier contracts in the US) to drastically cut down this loss margin.

## 🛠️ Tech Stack & Methodology
To conduct this analysis, the following tools and techniques were utilized:
- **Data Cleaning & ETL:** Power Query
- **Data Modeling:** Building a relational data model (One-to-Many relationships)
- **Calculations:** DAX (Using `CALCULATE` to isolate wasted shipping costs)
- **Visualization:** Power BI (Designing an interactive management dashboard in "Dark Mode" with a strong focus on UI/UX and scannability)

## 📂 Files in this Repository
- `Amazon_Sales.pbix` (The Power BI project file including the complete data model)
- `Amazon Sales.csv` (The underlying raw dataset)
