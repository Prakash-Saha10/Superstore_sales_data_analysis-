# 🚀 Superstore Sales Analysis

This project analyzes a **Superstore dataset** using Python, Pandas, Matplotlib, and Seaborn to explore revenue, customers, products, and time trends.  
The workflow covers **data cleaning → exploration → aggregation → visualization → insights.**

---

## 📊 Key Analysis Performed

### 1️⃣ Basic Exploration
- Dataset shape, data types, and missing values
- Count of unique customers, orders, and products
- Top 10 cities by number of orders
- Revenue per row, with mean/min/max revenue per order

### 2️⃣ Data Cleaning
- Removed duplicates and invalid rows (negative quantity or price)
- Converted dates (`Order Date`, `Ship Date`) to datetime
- Standardized text columns (segment, ship mode)
- Removed rows with missing `Customer ID`

### 3️⃣ Aggregation & Grouping
- Total revenue per customer (top 5 customers)
- Revenue per customer segment (bar chart)
- Average order value per country
- Top 10 cities by revenue (bar chart)
- Monthly revenue trends (line chart)

### 4️⃣ Time Series Analysis
- Orders per month (line chart)
- Monthly revenue peaks (November 2017 highest sales)
- Average shipping time (~3.97 days)
- Repeat customers (multiple orders across months)

### 5️⃣ Customer & Product Insights
- Top 10 products by revenue
- Least selling products
- Average revenue per order per segment
- Common shipping mode per segment
- Revenue contribution by top 20% customers (Pareto rule)

### 6️⃣ Visualization
- Bar chart of revenue per segment
- Boxplot of revenue distribution by segment
- Correlation heatmap (Quantity, Unit Price, Revenue)
- Scatter plot of Quantity vs Revenue (by segment)
- Line plot of monthly revenue with annotations

---

## ⚙️ Tech Stack
- **Python** 🐍
- **Pandas & NumPy** → Data cleaning & analysis
- **Matplotlib & Seaborn** → Visualizations

---

## 📷 Sample Visuals
- 📈 Monthly Revenue Trend  
- 📊 Revenue by Segment  
- 🔥 Top 10 Cities by Revenue  
- 📦 Revenue Distribution per Segment  
- 📉 Correlation Heatmap  

---

## 🚀 Run the Project

```bash
# 1. Clone this repo
git clone https://github.com/your-username/superstore-analysis.git

# 2. Enter project folder
cd superstore-analysis

# 3. Install dependencies
pip install pandas numpy matplotlib seaborn

# 4. Run the script
python superstore_analysis.py
