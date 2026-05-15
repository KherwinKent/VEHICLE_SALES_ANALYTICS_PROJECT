# Vehicle Sales Analytics Project Documentation

Data Collection, Preprocessing, EDA, Modeling, Dashboard, Insights, and Recommendations
Project Dataset: Vehicle Sales / Car Prices Dataset
Tool Used: Microsoft Power BI Desktop
Main Table: Fact_Car_Sales
Dashboard Theme: Vehicle Sales Analytics Dashboard
Project Summary
This project analyzes vehicle sales data using Power BI. I cleaned the vehicle sales dataset, created a fact table and dimension tables, built KPI measures, created EDA visuals, and developed an interactive dashboard. The analysis follows the required frameworks: CLEAN Framework for preprocessing, Pyramid Framework for key metrics and measures, Star Schema for data modeling, and DASH Framework for dashboard design.
2.1 Data Collection
For data collection, I used a real-world vehicle sales dataset in CSV format. The dataset contains vehicle transaction records with fields such as year, make, model, trim, body type, transmission, VIN, state, condition, odometer, color, interior, seller, MMR, selling price, and sale date.
Requirement
How It Was Addressed
Real-world dataset
Used a vehicle sales/car prices dataset from Kaggle.
Data format
CSV file imported into Power BI.
Minimum 100,000 records
The loaded fact table contains 558,837 rows, which satisfies the requirement.
Dashboard suitability
The dataset supports sales analysis, vehicle analysis, seller/location analysis, and time-based trends.

2.2 Data Preprocessing Using the CLEAN Framework
I cleaned the dataset before dashboarding to make sure that the data was readable, consistent, and ready for Power BI analysis. I followed the CLEAN Framework to document the preprocessing process in a simple and organized way.
CLEAN Step
What I Did
C - Correct Inconsistencies
I standardized text formatting, capitalized words properly, cleaned seller names, and converted state abbreviations into full state names such as FL to Florida and CA to California.
L - Locate Missing Values
I checked the dataset for blank, null, and invalid values. Missing or null values were replaced with a dash (-) so every record still has a readable value.
E - Eliminate Duplicates
I removed duplicate records where needed and avoided deleting important transactional records from the fact table. For dimension tables, I removed duplicate combinations only after creating the correct dimension structure.
A - Adjust Data
I formatted date values into a readable format like January 29, 2015, 4:30 a.m. PST. I also formatted numeric values professionally while keeping their original meaning.
N - Normalize and Finalize
I prepared the dataset for Power BI by creating clean tables, using consistent column names, and building dimension tables for data modeling.

Important preprocessing decisions:
I did not normalize prices into a 0 to 1 scale because selling prices, MMR, odometer, and costs should stay in their real-world values for dashboard interpretation.
I kept the fact table as the transactional table because each row represents a vehicle sale record.
I created dimension tables from the fact table to support Star Schema modeling.
2.3 Exploratory Data Analysis (EDA)
For the EDA part, I generated summary statistics and created KPI measures in Power BI. I followed the Pyramid Framework by placing the most important business metrics at the top, supporting visuals in the middle, and detailed analysis at the bottom.
KPI / Measure
Purpose
Total_Sales
Shows the total vehicle sales revenue.
Total_Vehicles_Sold
Counts the number of vehicles sold using VIN.
Average_Selling_Price
Shows the average vehicle selling price.
Average_MMR
Shows the average market value based on MMR.
Average_Odometer
Shows the average mileage of vehicles sold.
Max_Selling_Price
Shows the highest selling price in the dataset.
Min_Selling_Price
Shows the lowest selling price in the dataset.

Dashboard summary statistics used in the EDA:
Metric
Observed Dashboard Value
Total Sales
Approximately 7.61 billion
Total Vehicles Sold
Approximately 559K
Average Selling Price
Approximately 13.61K
Average MMR
Approximately 13.77K
Average Odometer
Approximately 68.32K
Max Selling Price
Approximately 64K
Min Selling Price
Approximately 200

Visualizations created:
KPI Cards for totals and averages.
Bar Chart for Total Sales by Make.
Line Graph for Total Sales by Sale Date.
Pie/Donut Chart for Count of VIN by Body Type.
Map Visual for Total Sales by State.
Table Visual for detailed records such as make, model, state, selling price, and seller.
Slicers for filtering by Make, State, Body, Transmission, Color, and Year.
Pyramid Framework: Key Metrics and Measures
Pyramid Level
Dashboard Elements
Purpose
Top Level - Key Metrics
Total Sales, Total Vehicles Sold, Average Selling Price, Average MMR, Average Odometer
Gives a quick executive summary of business performance.
Middle Level - Supporting Analysis
Sales by Make, Sales by Date, Sales by State, Body Type Distribution
Explains what factors affect the main KPIs.
Bottom Level - Detailed Analysis
Detailed transaction table and slicers
Allows users to investigate individual records and filter the dashboard.

2.4 Data Modeling / Analytics
For data modeling, I used a Star Schema. The center table is Fact_Car_Sales, and the dimension tables describe the sales records. I also started creating surrogate primary keys in Power Query so that each dimension table can connect properly to the fact table.
Table
Role
Main Fields / Keys
Fact_Car_Sales
Fact Table
VIN, Sellingprice, MMR, Odometer, Condition, SaleDate, Vehicle_ID, Location_ID, Appearance_ID, Time_ID
Dim_Vehicle_PQ
Dimension Table
Vehicle_ID, Make, Model, Trim, Body, Transmission
Dim_Location_PQ
Dimension Table
Location_ID, State, Seller
Dim_Appearance_PQ
Dimension Table
Appearance_ID, Color, Interior
Dim_Time_PQ
Dimension Table
Time_ID, SaleDate, Year

Analytics methods applied:
Star Schema for data modeling.
Descriptive analytics through summaries, averages, totals, rankings, and trends.
Trend analysis using the line graph for Total Sales by SaleDate.
Predictive analytics can be added through Power BI forecasting on the line graph once the date field is properly recognized as a real date/time column.
2.5 Visualization and Dashboard Using the DASH Framework
The dashboard was created in Power BI and designed to be interactive, readable, and useful for decision-making. I used the DASH Framework to organize the dashboard clearly.
DASH Step
How It Was Applied
D - Define the Goal
The dashboard answers the main question: How are vehicle sales performing across brands, states, body types, and time?
A - Arrange the Layout
KPI cards were placed at the top, analysis charts in the middle, and detailed tables/filters around the dashboard.
S - Show the Right Visuals
I used cards, bar charts, line graph, pie/donut chart, map visual, table visual, and slicers.
H - Highlight Insights
The most important metrics and patterns are visible through KPI cards, top-selling makes, sales trends, state performance, and body type distribution.

Dashboard components:
KPI cards: Total Sales, Total Vehicles Sold, Average Selling Price, Average MMR, Average Odometer, Max Selling Price, and Min Selling Price.
Filters/slicers: Make, State, Body, Transmission, Color, and Year.
Charts: Total Sales by Make, Total Sales by SaleDate, Count of VIN by Body, and Total Sales by State.
Detail table: Make, Model, State, Selling Price, and Seller.

2.6 Insights and Recommendations
Based on the dashboard results, I created the following insights and recommendations. These are written in a practical business context so they can be explained naturally during presentation.
Insight
Evidence from Dashboard
Recommendation
1. Ford appears to be the strongest brand by sales.
The Total Sales by Make bar chart shows Ford as the top-performing make compared with other brands.
The business should prioritize Ford inventory and analyze which Ford models produce the highest revenue.
2. Average selling price is slightly lower than average MMR.
Average Selling Price is about 13.61K while Average MMR is about 13.77K.
Review pricing strategy because some vehicles may be selling below estimated market value. This can help improve profit margins.
3. Vehicle mileage is high on average.
Average Odometer is about 68.32K miles.
Segment vehicles by mileage range to understand how mileage affects selling price and buyer demand.
4. Sedan and SUV body types dominate the vehicle records.
The Count of VIN by Body visual shows major body categories such as Sedan and SUV.
Focus marketing and inventory planning around high-demand body types, while monitoring lower-demand categories.
5. Sales performance varies by state and seller.
The map and detail table show differences in sales by state and seller.
Compare seller performance by location and identify which states or sellers produce stronger revenue.

Real-World Interpretation
In a real business setting, this dashboard can help a vehicle dealership, auction company, or vehicle resale business understand where sales are strongest, which brands perform best, and how pricing compares with market value. The dashboard can also support inventory planning, pricing decisions, and seller performance evaluation.
Complete Process Summary
Project Phase
What I Created
Data Collection
Collected and imported a real-world vehicle sales CSV dataset with over 100,000 records.
Data Preprocessing
Cleaned missing values, duplicates, text formatting, state names, seller names, date formatting, and column formatting using the CLEAN Framework.
EDA
Created KPI measures, summary statistics, bar chart, line graph, pie/donut chart, map, table, and filters using the Pyramid Framework.
Data Modeling
Built a Star Schema with Fact_Car_Sales and dimension tables such as Dim_Vehicle, Dim_Location, Dim_Appearance, and Dim_Time.
Dashboard
Developed an interactive Power BI dashboard using KPI cards, filters, charts, and a clean layout based on the DASH Framework.
Insights
Generated actionable insights and recommendations based on sales, pricing, vehicle type, mileage, brand, and location patterns.




