This project focuses on analyzing pizza sales data to uncover valuable insights into business performance using SQL, Power BI, and Power Query. The analysis highlights key performance indicators (KPIs), sales trends, and customer preferences to support data-driven decision-making.

📁 Project Structure
pizza_sales.csv – Raw pizza sales dataset.

Pizza_dashboard2.pbix – Power BI dashboard file.

Pizza Sales Data Analysis Project Documentation.docx – Full project documentation.

README.md – Project overview.

🎯 Objective
To analyze pizza sales data to answer business-critical questions such as:

What is the total revenue?

What are the most and least popular pizzas?

What days or months have the highest order volumes?

Which pizza size or category is the most profitable?

📊 Key Metrics
The project evaluates the following metrics:

Total Revenue

Average Order Value

Total Pizzas Sold

Total Orders

Average Pizzas Per Order

🧮 Data Processing
Data Import: Imported from Excel into a MySQL database.

SQL Analysis: Queries were written to extract KPIs and trends.

Power BI: Used for advanced visualization and insights.

Power Query: Applied for data cleaning and transformation.

🧠 SQL Insights
Example Queries:

Total Revenue:

sql
Copy
Edit
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;
Average Order Value:

sql
Copy
Edit
SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_order_Value FROM pizza_sales;
Top 5 Pizzas by Revenue:

sql
Copy
Edit
SELECT TOP 5 pizza_name, SUM(total_price) AS Total_Revenue
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Revenue DESC;
More queries in the documentation.

📈 Power BI Dashboard
Visualizations include:

Daily & Monthly Order Trends

Sales % by Pizza Category & Size

Best & Worst Selling Pizzas

Category-wise Pizza Sales

🧼 Data Cleaning
Performed using Power BI’s Power Query:

Removed nulls

Standardized date/time formats

Created conditional and custom columns

✅ Conclusion
This project enabled:

Identifying top-performing pizzas and categories

Recognizing slow-moving products

Understanding customer order behavior

Enhancing business decision-making with real data

🛠 Tech Stack
SQL (MySQL)

Power BI

Power Query

Excel

📌 How to Run
Clone the repository.

Open Pizza_dashboard2.pbix in Power BI.

Connect your MySQL data source or use the provided pizza_sales.csv.

Explore and interact with the dashboard!

📬 Contact
For questions or feedback, feel free to reach out via GitHub Issues.
