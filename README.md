# 🧠 Product Sales Data Analysis

## 📋 Overview
This project analyzes product sales data to identify key business insights, sales trends, and performance metrics.  
It demonstrates a full **data analytics pipeline** — loading raw CSV files, cleaning and transforming data, exploring patterns using Python, and preparing it for visualization in Power BI and SQL analysis.  

---

## 📊 Dataset
- **Source:** Monthly sales CSV files (combined into a single dataset)
- **Rows:** ~186,850  
- **Columns include:**
  - `Order ID` — Unique identifier for each order  
  - `Product` — Product name  
  - `Quantity Ordered` — Units sold  
  - `Price Each` — Price per unit  
  - `Order Date` — Purchase timestamp  
  - `Purchase Address` — Customer location  

**Feature Engineering:**
- Extracted **Month** and **City** from `Order Date` and `Purchase Address`  
- Calculated **Sales = Quantity Ordered × Price Each**  
- Converted columns to correct data types (`int`, `float`, `datetime`)  
- Removed duplicates and handled missing values  

---

## 🧰 Tools & Technologies
| Tool | Purpose |
|------|----------|
| **Python (Pandas, NumPy, Matplotlib, Seaborn)** | Data cleaning, transformation, and exploratory data analysis |
| **SQL (PostgreSQL / MySQL / SQL Server)** | Running analytical queries and aggregations |
| **Power BI** | Building an interactive dashboard for sales insights |
| **Gamma App** | Creating final presentation slides |
| **Jupyter Notebook** | Documenting the analytical workflow |

---

## 🔍 Project Steps

### 1️⃣ Data Loading
- Imported multiple `.csv` files using `os` and combined them into a single DataFrame with **Pandas**.  
- Verified file integrity and previewed random samples to ensure consistency.

### 2️⃣ Data Cleaning
- Removed **545 rows** containing missing (`NaN`) data.  
- Resolved incorrect entries (e.g., rows with `"Quantity Ordered"` as text).  
- Replaced invalid string entries with column averages.  
- Converted:
  - `Quantity Ordered` → **integer**  
  - `Price Each` → **float**  
  - `Order Date` → **datetime**  
- Removed duplicates and ensured uniform formatting.

### 3️⃣ Feature Engineering
- Created new derived columns:
  - `Month` — extracted from `Order Date`  
  - `City` — extracted from `Purchase Address`  
  - `Sales` — calculated as `Quantity Ordered × Price Each`  

### 4️⃣ Exploratory Data Analysis (EDA)
- Identified total and average monthly sales  
- Found top-selling products and high-performing cities  
- Analyzed monthly revenue trends and correlations  
- Visualized results using Matplotlib and Seaborn  

### 5️⃣ SQL Analysis
Performed advanced queries for:
- **Monthly sales performance**
- **Top 10 cities by revenue**
- **Most profitable products**
- **Average sales per order**

### 6️⃣ Power BI Dashboard
- Built an interactive Power BI dashboard with:
  - **KPIs:** Total Sales, Profit, Orders  
  - **Visuals:** Monthly trends, Product comparison, Regional sales  
  - **Filters:** Month, Product, and City  

### 7️⃣ Presentation & Reporting
- Summarized the findings in a clear, business-focused **report**  
- Created an interactive presentation using **Gamma App**

---

## 📈 Dashboard
The Power BI dashboard highlights:
- Total revenue and order volume  
- Monthly sales performance  
- Top 10 cities and best-selling products  
- Interactive slicers for better exploration  

*(Add dashboard screenshot or link here)*

---

## 📊 Key Insights
- **December** recorded the highest total sales.  
- **MacBook Pro** and **iPhone** ranked as top-selling products.  
- **San Francisco** and **Los Angeles** generated the highest regional revenue.  
- Strong positive correlation between **discounts and order volume**.  

---

