# Virtual Internship Experience (VIX) Bank Muamalat X Rakamin Academy
This project is created to complete the final task on Internship Experience (VIX) of The Bank Muamalat Batch Juli 2023 in collaboration with Rakamin Academy (Edutech Company)

# Objective
The purpose of this project is to analyze the characteristics of digital users regarding sales. This type of analysis is to create a visualization in the form of a company sales dashboard from data consisting of several tables. The tool used for visualization is Looker Studio. The visualization has following objective:
-Total sales

-Total sales by product category name

-Total quantity by product category name

-Total sales by city

-Total quantity by city

-top 5 product categories with the highest sales

-top 5 product categories with the highest quantity 

# Dataset
-Customers

-Orders

-ProductCategory

-Product

# Entity Relationship Diagram
![image](https://github.com/rachman777/vix_businessintelligence/assets/142157665/0bd67e84-c3b2-4524-905c-fb6099428683)


# Master Table
SELECT Orders.Date,ProductCategory.CategoryName, Products.ProdName, Products.Price, Orders.Quantity, [Price]*[Quantity] AS [Total Sales], Customers.CustomerEmail, Customers.CustomerCity
                  
FROM ProductCategory 

INNER JOIN (Products INNER JOIN (Customers INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID) ON Products.ProdNumber = Orders.ProdNumber) ON ProductCategory.CategoryID = Products.Category;
![image](https://github.com/rachman777/vix_businessintelligence/assets/142157665/0410e897-1f69-4280-a87e-c520ab2c62ae)

# Sales Report
![image](https://github.com/rachman777/vix_businessintelligence/assets/142157665/53bde656-ce1c-456a-9ac4-3f600bf27b11)

-The total sales of all products amounted to $1,754,750.57. 

-The product category in the form of Robots provides the company with the highest sales with $743,500.

-eBooks was the most purchased in quantity, with 3,123.

-Customers From Washington give biggest total of sales than other city

-Same as total sales, customers from wahington have biggest quantity of product purchase

# recommendation
-Make bundling of robots and drone products as products with the largest total sales with the kit so that it can further boost sales of the kit.

-Make a bundling of the ebook product as the product with the largest sales volume with training videos and blueprints so that can further increase the sales quantity of the product.

-Maintaining existing sales in Washington with regular advertising or providing discounts and creating marketing collaborations with other companies where when customers buy PT Sejahtera Bersama products they will get discount vouchers that can be spent elsewhere.

-Create a massive marketing campaign in cities with big potential such as Houston and San Diego.







