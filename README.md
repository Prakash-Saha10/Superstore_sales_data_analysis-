🚀 Superstore Sales Analysis
This project dives deep into a Superstore's sales data, using Python's data-savvy libraries to unearth actionable insights. We're talking Pandas for the heavy lifting, and Matplotlib & Seaborn to make the numbers look good. 📊

🎯 The Mission: Uncover the 'Why' Behind the 'What'
Our goal was simple: turn raw data into a story. We focused on three core questions:

💰 Revenue & Sales: What's the money-making narrative?

🧑‍🤝‍🧑 Customer Behavior: Who are our VIPs and what makes them tick?

📦 Product & Operations: What are we selling, and how efficiently are we shipping it?

💡 Top-Tier Insights
💰 Revenue & Sales
Total Haul: A whopping $1.8M in total revenue after cleanup.

The Big Month: Sales hit their all-time high in November 2017, peaking at $95,951.

City Giants: New York City and Los Angeles are our revenue champions, proving geography is key.

Top 10 Cities by Revenue

Python

df.groupby('City')['Revenue'].sum().sort_values(ascending=False).head(10)
🧑‍🤝‍🧑 Customer Behavior
Segment Kings: The Consumer segment is the most profitable by a landslide.

The 80/20 Rule: Our top 20% of customers are generating a massive chunk of total revenue.

Revenue by Customer Segment

Python

revenue_per_segment.plot(kind='bar')
📦 Product & Operations
Star Products: The Canon imageCLASS 2200 Advanced Copier and GBC Ibimaster 5000 Pro binding machine are our top sellers. They're basically printing money for us.

Slow Movers: Certain fasteners and supply items aren't pulling their weight. Time to re-evaluate their stock.

Shipping Speed: On average, an order gets to the customer in about 3.97 days. Not bad!

⚙️ The Technical Stack
We used a standard data science workflow:

Data Wrangling:

df.drop_duplicates() to kick out the clutter.

pd.to_datetime() to make sure our dates behave.

.str.lower() and .str.strip() to keep our text data clean and consistent.

Aggregation & Grouping:

df.groupby() was our go-to for summing up sales by city, segment, and product.

Time Series:

We used df.set_index('Order Date') and .resample('M') to track sales over time. This let us pinpoint that November 2017 peak.

Monthly Sales Trend

Python

monthly_sales.plot(title="Monthly Revenue Trend", marker='o')
Visualization:

Seaborn's heatmap() confirmed a strong positive correlation between Quantity, Unit Price, and Revenue. More product and higher prices mean more cash.

Boxplots helped us visualize the distribution of revenue across different customer segments.

🚀 Get the Code Running
Want to see the magic yourself? It's easy.

Bash

# 1. Clone the repo
git clone https://github.com/your-username/superstore-analysis.git

# 2. Get inside the folder
cd superstore-analysis

# 3. Install the dependencies
pip install -r requirements.txt

# 4. Run the script
python superstore_analysis.py
superstore.csv must be in the same directory. Happy coding! 💻
