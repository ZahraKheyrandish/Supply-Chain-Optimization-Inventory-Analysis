
#  Supply Chain Optimization: Simulated Pharmaceutical Network

## Project Objective
This project simulates a pharmaceutical supply chain network and performs data-driven analysis to uncover inefficiencies, identify performance bottlenecks, and provide actionable insights. Through detailed EDA and visualization, we aim to support better decision-making for procurement, inventory, and distribution strategies.

---

##  Data Source
A synthetic dataset was created to mimic a realistic supply chain environment with 10 warehouses, multiple suppliers, and thousands of pharmaceutical products. The dataset includes:
- **Product Details**
- **Sales Transactions**
- **Inventory Levels**
- **Suppliers and Delivery Data**

---

##  Tools Used
- **Python** for simulation, data analysis, and visualization
- **Pandas & NumPy** for data manipulation
- **Matplotlib & Seaborn** for visualizations
- **Google Colab** as the development environment

---
##  Dashboard:

To provide a dynamic and user-friendly interface for exploring the project's findings, an interactive dashboard was built using Streamlit. You can access the live dashboard here: [Launch Dashboard.](https://supply-chain-optimization-inventory-analysis-jpfxbgrucyvvvjftv.streamlit.app/#total-cost-by-supplier)


Filter data by region and total cost to focus on specific segments of the supply chain.

View key performance indicators (KPIs) and visualizations, including total cost by supplier, quantity shipped by category, and monthly sales trends.

Interact with a Lead Time Prediction Model to forecast delivery times for new orders

---
##  Exploratory Data Analysis (EDA)

### 1. Monthly Sales Trend
![Monthly Sales](Plots/download%20(51).png)

This line chart visualizes monthly sales across the simulation. Sales peak during winter months and drop in summer—common in real-world pharmaceutical trends.

---

### 2. Sales by Product Category
![Sales by Category](Plots/download%20(50).png)

A bar chart displaying total sales across top product categories. Vitamins, antibiotics, and chronic condition medications lead in revenue.

---

### 3. Supplier Performance
![Supplier Performance](Plots/download%20(49).png)

A scatter plot showing average lead time vs. delivery delay rate per supplier. Bubble size indicates number of orders. Top-left suppliers are ideal: fast and reliable.

---

### 4. Unit Price Distribution
![Unit Price Distribution](Plots/download%20(48).png)

Histogram of product unit prices. Right-skewed distribution—most products are moderately priced, with a few high-cost items (e.g., specialty drugs).

---

### 5. Distribution of Sold Quantities
![Quantity Distribution](Plots/download%20(47).png)

Most sales are in low quantities, consistent with pharmacy ordering behavior—frequent and in small batches.

---

### 6. Overall Sales Trend
![Overall Sales](Plots/download%20(46).png)

Line plot of total daily sales across the simulation. Seasonal spikes reflect demand cycles.

---

### 7. Top 10 Bestselling Products
![Top 10 Products](Plots/download%20(45).png)

Bar chart showing top 10 products by unit sales. These products are critical to inventory planning.

---

### 8. Waste and Stockouts Analysis
![Waste and Stockouts](Plots/download%20(44).png)

Dual subplot:
- **Top:** Waste due to expiration. Certain slow-moving products are consistently wasted.
- **Bottom:** Frequency of stockouts by product. Highlights under-forecasted items.

---

## 📌 Key Takeaways
- **Seasonality** drives significant sales variation.
- **Inventory waste** is concentrated in specific SKUs—suggests overstocking.
- **Supplier delays** vary widely—room for performance-based contracting.
- **Top-selling products** account for the majority of demand—prioritize them.

---

##  Next Steps (Future Work)
- Simulate disruptions (e.g., supplier failure) to test network resilience
- Model safety stock levels using statistical methods
- Build predictive models for sales forecasting
- Optimize reorder points and economic order quantity (EOQ)

---

##  Goal
This project demonstrates how simulation and analytics can be applied to a synthetic supply chain for actionable insights. With enhanced forecasting and data-driven procurement, such a system can reduce waste, improve service levels, and streamline operations.
