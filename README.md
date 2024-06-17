# "Analyzing the Impact of Product Visibility and Price on Sales Using Machine Learning"

# Project Overview:
This project aims to analyze and predict the impact of product visibility and price on sales across different outlet types using machine learning models. It investigates how these relationships vary based on outlet characteristics such as size, year of establishment, and location.

# Project Objectives:
1.	To evaluate the impact of product visibility and price on sales across various outlet types:
Method: Descriptive statistics and Regression Analysis.
Descriptive statistics will summarize and provide insights into the data’s structure and Regression analysis will determine how product visibility (Item_Visibility) and pricing (Item_MRP) influence sales (Item_Outlet_Sales) across various outlet types (Outlet_Type). This will help to identify the individual and combined effects on sales performance.
2.	To examine the moderating effects of outlet characteristics on sales dynamics:
Method: Interaction effect analysis with multiple regression models.
Interaction effect analysis with multiple regression models will investigate how outlet characteristics influence the relationship between product visibility, pricing and sales. By implementing this, the study will assess how size (Outlet_Size), year of establishment (Outlet_Establishment_Year), and location (Outlet_Location_Type) affect the link between product visibility, pricing, and sales.
3.	To create tailored sales optimisation strategies based on outlet attributes:
Method: Machine learning models (e.g., decision trees, random forests) 
Machine learning models such as decision trees, random forests and XGBoost help to forecast sales and determine critical areas for optimisation. The insights gained from this analysis will help to develop customized strategies tailored to each outlet's characteristics, such as type, size, establishment year, and location.


# Summary of Project and Background:
BigMart, a large retail chain, operates multiple stores across various cities. To enhance its operations, BigMart aims to understand and predict the sales patterns of different products in various stores. The dataset at hand contains sales data from 2013 for 1559 products across 10 different stores. Each product and store is described by several attributes, which include both categorical and numerical features that cover aspects like product visibility, pricing, outlet size, the year the outlet was established, and its location. 
This study seeks to investigate the impact of product visibility and price on sales across various retail outlet types, as well as how these connections are modified by outlet-specific features such as size, year of establishment, and location. Retailers confront major hurdles in optimising product positioning and pricing strategies to maximise sales (Baker, Grewal, & Parasuraman 1994). Understanding these dynamics can result in more successful and targeted marketing efforts. Previous research has demonstrated that product exposure and pricing are important elements in influencing customer purchase behaviour (Chandon, Hutchinson, Bradlow, & Young, 2009; Inman, Winer, & Ferraro, 2009). However, more detailed research is required, considering the moderating impact of outlet characteristics.
Using data from the BigMart retail chain, regression analysis will determine the primary impacts of product visibility and pricing on sales. An interaction effect study will determine how outlet size, establishment year, and location affect these associations. This research will give merchants practical information to improve their sales strategy, resulting in greater performance and customer satisfaction. The findings will give a thorough knowledge of the complex interaction between product visibility, price, and outlet features, as well as practical insights for optimising retail strategy in a variety of market scenarios.


# Dataset: 
The dataset used for this project is taken from Kaggle and is provided in CSV format. The training dataset contains 8,523 records and the test dataset contains 5,681 records
Link to the dataset: https://www.kaggle.com/datasets/uniabhi/bigmart-sales-data

The following are the key features:

•	Item_Identifier: Distinct identifier for each product.

•	Item_Weight: Weight of each product.

•	Item_Fat_Content: Indicates whether the product is of low fat or regular.

•	Item_Visibility: The percentage of the total display area allocated to this product in a store.

•	Item_Type: Indicates the product's category.

•	Item_MRP: Maximum Retail Price (list price) of the product.

•	Outlet_Identifier: Distinct identifier for each store.

•	Outlet_Establishment_Year: The year in which the store was founded.

•	Outlet_Size: Size of the store (Small, Medium, High).

•	Outlet_Location_Type: Type of city in which the store is located (Tier 1, Tier 2, Tier.

•	Outlet_Type: Type of store (e.g., Supermarket Type1, Grocery Store).

•	Item_Outlet_Sales: Sales of each product in the particular store (target variable).

