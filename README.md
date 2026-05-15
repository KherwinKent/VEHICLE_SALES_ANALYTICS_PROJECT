<div align="center">

# 🚘 VEHICLE SALES ANALYTICS DASHBOARD

### 📊 Power BI Business Intelligence Project

<img src="https://img.shields.io/badge/PowerBI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/Dataset-558K_Records-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Project-Completed-success?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Frameworks-CLEAN%20%7C%20PYRAMID%20%7C%20DASH-darkblue?style=for-the-badge"/>

<br><br>

## 🚗 Overview of Vehicle Sales Performance Using Power BI

A complete Business Intelligence dashboard project focused on:
Vehicle Sales Analysis, Data Cleaning, Exploratory Data Analysis (EDA), Star Schema Modeling, KPI Visualization, and Business Insights.

</div>

---

# 📌 PROJECT OVERVIEW

This project analyzes a real-world vehicle sales dataset using **Microsoft Power BI Desktop**.  
The goal of the project is to transform raw vehicle transaction data into a professional and interactive dashboard that provides valuable business insights.

The dashboard helps analyze:

✅ Vehicle sales performance  
✅ Brand performance  
✅ Seller and location analysis  
✅ Pricing analysis  
✅ Mileage trends  
✅ Vehicle body type distribution  
✅ Time-based sales trends  

---

# 🖼 DASHBOARD PREVIEW

> 📌 Upload your dashboard screenshot to GitHub and replace the image link below.

<p align="center">
<img src="YOUR_DASHBOARD_IMAGE_LINK_HERE" width="100%">
</p>

---

# 🛠 TOOLS & TECHNOLOGIES USED

| Tool | Purpose |
|---|---|
| Microsoft Power BI | Dashboard Development |
| Power Query | Data Cleaning & Transformation |
| DAX | KPI Measures & Calculations |
| CSV Dataset | Data Source |
| GitHub | Documentation & Version Control |

---

# 📂 DATASET INFORMATION

| Requirement | Description |
|---|---|
| Dataset Name | Vehicle Sales / Car Prices Dataset |
| Dataset Source | Kaggle |
| Dataset Type | Real-world Dataset |
| File Format | CSV |
| Total Records | 558,837 Rows |
| Main Fact Table | Fact_Car_Sales |

---

# 🧹 DATA PREPROCESSING  
## CLEAN FRAMEWORK IMPLEMENTATION

The dataset was cleaned and prepared before dashboard development.

---

## ✅ C — Correct Inconsistencies

- Standardized seller names
- Cleaned text formatting
- Converted abbreviations into readable formats
- Corrected inconsistent state names

### Example:
- FL → Florida
- CA → California

---

## ✅ L — Locate Missing Values

- Checked for blank and null values
- Replaced missing values using readable placeholders

### Example:
- Null → "-"

---

## ✅ E — Eliminate Duplicates

- Removed duplicate dimension records
- Preserved important transactional records in the fact table

---

## ✅ A — Adjust Data

- Formatted dates properly
- Adjusted numerical formats
- Improved readability of values

### Example:
- January 29, 2015, 4:30 a.m. PST

---

## ✅ N — Normalize & Finalize

- Created clean dimension tables
- Finalized Star Schema structure
- Standardized naming conventions

---

# 🏗 DATA MODELING  
## STAR SCHEMA IMPLEMENTATION

The project follows a **Star Schema** data model for better performance and scalability.

---

## ⭐ FACT TABLE

### Fact_Car_Sales

Contains:
- Vehicle transactions
- Selling price
- MMR
- Odometer
- Condition
- Sale date
- Foreign keys

---

## ⭐ DIMENSION TABLES

| Dimension Table | Purpose |
|---|---|
| Dim_Vehicle_PQ | Vehicle details |
| Dim_Location_PQ | Seller & state information |
| Dim_Appearance_PQ | Color & interior details |
| Dim_Time_PQ | Date and year analysis |

---

# 🔑 SURROGATE PRIMARY KEYS

To support proper table relationships, surrogate primary keys were created in Power Query.

### Example Keys:
- Vehicle_ID
- Location_ID
- Appearance_ID
- Time_ID

These keys were merged back into the fact table to establish relationships between dimensions and transactional data.

---

# 📈 EXPLORATORY DATA ANALYSIS (EDA)

The project follows the **PYRAMID FRAMEWORK** by organizing the dashboard into:

1. Key Metrics
2. Supporting Analysis
3. Detailed Analysis

---

# 📊 KPI MEASURES

| KPI Measure | Purpose |
|---|---|
| Total Sales | Overall revenue |
| Total Vehicles Sold | Number of vehicles sold |
| Average Selling Price | Average selling value |
| Average MMR | Average market value |
| Average Odometer | Average mileage |
| Max Selling Price | Highest vehicle sale |
| Min Selling Price | Lowest vehicle sale |

---

# 📉 VISUALIZATIONS USED

✅ KPI Cards  
✅ Bar Charts  
✅ Line Graphs  
✅ Donut Charts  
✅ Map Visuals  
✅ Table Visuals  
✅ Interactive Slicers  

---

# 🎨 DASHBOARD DESIGN  
## DASH FRAMEWORK IMPLEMENTATION

The dashboard was designed using the **DASH Framework**.

---

## 🎯 D — Define the Goal

The dashboard answers:

> “How are vehicle sales performing across brands, states, body types, and time?”

---

## 🧩 A — Arrange the Layout

Dashboard sections were organized into:
- KPI Area
- Analysis Area
- Detailed Table Area
- Interactive Filter Area

---

## 📊 S — Show the Right Visuals

The dashboard includes:
- Cards
- Charts
- Maps
- Tables
- Filters

---

## 💡 H — Highlight Insights

The dashboard highlights:
- Best-selling brands
- Sales trends
- Regional sales performance
- Vehicle distribution
- Seller analysis

---

# 💡 INSIGHTS & RECOMMENDATIONS

---

## 🚗 1. Ford Generated the Highest Sales

### Insight:
Ford appears as the top-performing vehicle brand.

### Recommendation:
Increase Ford inventory and analyze high-performing Ford models.

---

## 💰 2. Selling Prices Are Slightly Lower Than MMR

### Insight:
Average Selling Price is lower than Average MMR.

### Recommendation:
Review pricing strategies to improve profit margins.

---

## 🛣 3. Vehicles Have High Average Mileage

### Insight:
Average odometer reading is high.

### Recommendation:
Segment vehicles based on mileage ranges for targeted marketing.

---

## 🚙 4. Sedan and SUV Dominate the Market

### Insight:
Sedan and SUV body types dominate vehicle sales.

### Recommendation:
Focus inventory and promotions on high-demand body types.

---

## 🌎 5. Sales Performance Varies by State

### Insight:
Some states and sellers outperform others.

### Recommendation:
Analyze high-performing regions and optimize regional inventory distribution.

---

# 🌍 REAL-WORLD BUSINESS INTERPRETATION

This dashboard can help:
- Vehicle dealerships
- Auto auction companies
- Car resale businesses

make better decisions regarding:
- Inventory management
- Pricing strategies
- Seller evaluation
- Sales forecasting
- Regional sales optimization

---

# 👨‍💻 PROJECT DEVELOPER

<div align="center">

# 🚀 DELA ROSA, KENT KHERWIN | CONCEPCION, JUSTINE | QUIROZ, BENEDICT | LUMANOG, PAULO | PINTOR, EDRICK JOHN

### Vehicle Sales Analytics Dashboard Project

📊 Microsoft Power BI Developer  
📈 Data Analytics Enthusiast  
🚗 Business Intelligence Project

</div>

---

# ⭐ PROJECT STATUS

✅ Data Collection Completed  
✅ Data Cleaning Completed  
✅ Star Schema Completed  
✅ Dashboard Completed  
✅ KPI Measures Completed  
✅ Insights & Recommendations Completed  

---

<div align="center">

# 🌟 THANK YOU FOR VIEWING THIS PROJECT 🌟

</div>
