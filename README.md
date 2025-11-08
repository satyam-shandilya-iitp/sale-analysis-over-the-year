# 🧠 Product Sales Data Analysis

## 📋 Overview
This project performs an in-depth **sales analysis** on product transaction data to uncover business insights, sales trends, and growth opportunities.  
It covers the full data analytics workflow — from data ingestion and cleaning to exploratory analysis, SQL querying, and Power BI dashboard creation.  
The goal is to help stakeholders make data-driven decisions by visualizing sales performance and identifying top-performing products and regions.

---

## 📊 Dataset
- **Source:** Internal sales CSV files (multiple monthly datasets combined)
- **Size:** ~186,850 rows  
- **Key Columns:**
  - `Order ID` — Unique identifier for each transaction  
  - `Product` — Product name sold  
  - `Quantity Ordered` — Number of units purchased  
  - `Price Each` — Unit price of the product  
  - `Order Date` — Date and time of the purchase  
  - `Purchase Address` — Customer’s shipping address  

**Feature Engineering:**
- Extracted **Month**, **City**, and **Sales (Quantity × Price)** columns  
- Cleaned and standardized data types  
- Removed duplicates and missing entries  

---

## 🧰 Tools & Technologies
| Tool | Purpose |
|------|----------|
| **Python (Pandas, NumPy, Matplotlib, Seaborn)** | Data cleaning, transformation, and EDA |
| **SQL (PostgreSQL / MySQL / SQL Server)** | Running analytical queries |
| **Power BI** | Creating interactive dashboards |
| **Gamma App** | Building the final presentation slides |
| **Jupyter Notebook** | Documenting the analysis workflow |

---

## 🔍 Project Steps

### 1️⃣ Data Loading
- Imported multiple CSV files using `os` and `pandas`
- Combined all files into one unified dataset (`All_data`)

### 2️⃣ Data Cleaning
- Removed **545 rows** with missing values  
- Fixed mixed-type errors (e.g., `"Quantity Ordered"` text values)
- Converted:
  - `Quantity Ordered` → integer  
  - `Price Each` → float  
  - `Order Date` → datetime  
- Removed duplicates and ensured consistent data types

### 3️⃣ Exploratory Data Analysis (EDA)
- Calculated total revenue and average order value  
- Found top-selling products by quantity and revenue  
- Identified best-performing months and cities  
- Visualized trends using Matplotlib & Seaborn

### 4️⃣ SQL Analysis
- Loaded cleaned data into SQL database  
- Queried:
  - Monthly sales trends  
  - Top 10 cities by total sales  
  - Products contributing most to revenue  
  - Profitability and quantity analysis  

### 5️⃣ Power BI Dashboard
- Built an interactive Power BI dashboard featuring:
  - KPIs: Total Sales, Orders, and Profit
  - Top Products & Cities
  - Monthly Revenue Trends
  - Filters for Month, City, and Product Category  

### 6️⃣ Reporting & Presentation
- Summarized findings in a concise **business report**  
- Created an **interactive presentation using Gamma App**

---

## 📈 Dashboard
The Power BI dashboard showcases:
- Total sales and profit overview  
- Top products and regions  
- Sales trend analysis by month  
- Interactive filters for better insight exploration  

*(Add screenshots here after uploading the `.pbix` file)*

---

## 📊 Key Insights
- **December** recorded the highest sales volume.  
- **MacBook Pro and iPhone** were top-selling products.  
- **San Francisco and Los Angeles** led total sales by city.  
- High correlation between **discounts and increased order volume**.

---



