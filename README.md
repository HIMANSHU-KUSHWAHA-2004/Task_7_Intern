<h1 style="font-family: Arial, sans-serif; color: #2c3e50;">TASK 7: Get Basic Sales Summary from a Tiny SQLite Database using Python</h1>

<p style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6; color: #333;">
This task analyzes the sales data of a small <strong>tech shop</strong>. Using Python and SQLite, we extract product-level 
sales insights — such as total units sold and total revenue — and display the results using both text output and a simple bar chart.
</p>

<h2 style="font-family: Arial, sans-serif; color: #34495e;">🎯 Objective</h2>
<p style="font-size: 16px; line-height: 1.6;">
Use SQL queries within Python to calculate key sales metrics from a tech shop database, and visualize the results using <code>matplotlib</code>.
</p>

<h2 style="font-family: Arial, sans-serif; color: #34495e;">🛠️ Tools Used</h2>
<ul style="font-size: 16px; color: #333;">
    <li>Python 3.x</li>
    <li>SQLite3 (for creating the database and running SQL)</li>
    <li>Pandas (for handling SQL query output)</li>
    <li>Matplotlib (for data visualization)</li>
</ul>

<h2 style="font-family: Arial, sans-serif; color: #34495e;">📦 Dataset</h2>
<p style="font-size: 16px;">
A small SQLite database named <code>sales_data.db</code> is created to represent the sales records of a tech shop. 
The <code>sales</code> table includes:
</p>
<ul style="font-size: 16px;">
    <li><strong>product</strong> – the name of the tech item (e.g. Laptop, Monitor)</li>
    <li><strong>quantity</strong> – number of units sold</li>
    <li><strong>price</strong> – unit price of the product</li>
</ul>

<h2 style="font-family: Arial, sans-serif; color: #34495e;">🚀 Deliverables</h2>
<ul style="font-size: 16px;">
    <li>A Python script or notebook that:
        <ul>
            <li>Connects to <code>sales_data.db</code></li>
            <li>Runs SQL to compute total quantity and revenue per product</li>
            <li>Displays the summary using <code>print()</code></li>
            <li>Plots a simple bar chart using <code>matplotlib</code></li>
        </ul>
    </li>
</ul>

<h2 style="font-family: Arial, sans-serif; color: #34495e;">📌 Sample SQL Logic</h2>
<pre style="background-color: #f4f4f4; padding: 15px; border-radius: 5px; font-size: 14px; font-family: Consolas, monospace; color: #2c3e50;">
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
</pre>

<h2 style="font-family: Arial, sans-serif; color: #34495e;">📈 Visualization</h2>
<p style="font-size: 16px;">
The output includes a bar chart titled <strong>Revenue by Product</strong>, saved as <code>sales_chart.png</code>. 
This chart gives a clear visual breakdown of which tech items generated the most revenue.
</p>

<p style="font-size: 14px; color: #7f8c8d;">
Author: Your Name - Himanshu Kushwaha | &nbsp; Dataset: Tech Shop Sales &nbsp; | &nbsp; Date: May 2025
</p>
