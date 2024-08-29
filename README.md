# "Analyzing the Impact of Product Visibility and Price on Sales Using Machine Learning"

# 1) Project Overview:
This project aims to analyze and predict the impact of product visibility and price on sales across different outlet types using machine learning models. It investigates how these relationships vary based on outlet characteristics such as size, year of establishment, and location.

# 2) Project Objectives:
The goal of this project is to leverage the Bigmart dataset to analyse and forecast item outlet sales. The specific objectives of the project are:
First Objective:
•	Analyze Sales Influencers: Identify and evaluate the impact of various factors such as product visibility, pricing and units sold on sales performance across different outlet types.
   o	Purpose: To gain actionable insights into how different attributes, including the newly calculated 'Units Sold' (which represents the number of units sold by dividing item outlet sales by item MRP) that affect sales. Understanding these dynamics will help inform more effective marketing and inventory strategies, thereby enhancing sales outcomes.
•	Examine Outlet Characteristics: Assess the influence of outlet attributes, includ-ing size, establishment year, and location, on sales performance.
   o	Purpose: To understand how these characteristics contribute to sales varia-tions, allowing for targeted improvements and optimized strategies based on outlet-specific factors.

Second Objective:
•	Moderation effects: Assess the interrelated effects of outlet size, year established and location with product visibility and pricing on sales performance
   o	 Purpose: To understand the impacts of different factors such as size, establish-ment year and location while interacting with one another on sales given a certain level of product visibility. An understanding of these moderating effects will pro-vide BigMart the flexibility required to shape their strategy in a way that leverages these dimensions, turning hindrances into opportunities for growth and optimiza-tion rather than relying on one-size-fits-all solution. If businesses have better un-derstanding of these traits, they could do marketing and pricing strategies accord-ing to the outlet for an improved sales income.

Third Objective:
•	Develop Predictive Models: Construct and refine predictive models to estimate Item_Outlet_Sales using available dataset attributes.
   o	Purpose: To enable accurate sales forecasting for new outlets, supporting ef-fective planning and inventory management by predicting future sales trends.


# 3) Summary of Project and Background:
BigMart, a large retail chain, operates multiple stores across various cities. To enhance its operations, BigMart aims to understand and predict the sales patterns of different products in various stores. The dataset at hand contains sales data from 2013 for 1559 products across 10 different stores. Each product and store is described by several attributes, which include both categorical and numerical features that cover aspects like product visibility, pricing, outlet size, the year the outlet was established, and its location. 
This study seeks to investigate the impact of product visibility and price on sales across various retail outlet types, as well as how these connections are modified by outlet-specific features such as size, year of establishment, and location. Retailers confront major hurdles in optimising product positioning and pricing strategies to maximise sales (Baker, Grewal, & Parasuraman 1994). Understanding these dynamics can result in more successful and targeted marketing efforts. Previous research has demonstrated that product exposure and pricing are important elements in influencing customer purchase behaviour (Chandon, Hutchinson, Bradlow, & Young, 2009; Inman, Winer, & Ferraro, 2009). However, more detailed research is required, considering the moderating impact of outlet characteristics.
Using data from the BigMart retail chain, regression analysis will determine the primary impacts of product visibility and pricing on sales. An interaction effect study will determine how outlet size, establishment year, and location affect these associations. This research will give merchants practical information to improve their sales strategy, resulting in greater performance and customer satisfaction. The findings will give a thorough knowledge of the complex interaction between product visibility, price, and outlet features, as well as practical insights for optimising retail strategy in a variety of market scenarios.


# 4) Code Functionality:

• Data Preprocessing: Cleans the data, handles missing values, encodes categorical variables, and normalizes the data.

• Feature Engineering: Creates new features to better capture the influences on sales such as 'Units Sold'.

• Model Training and Evaluation: Trains multiple regression models and evaluates them using metrics such as MSE (Mean Squared Error) and R² (Coefficient of Determination).

• Result Visualization: Generates plots to illustrate the actual versus predicted results and the learning curves for various models.

# 5) Input Data Format: 
The dataset used for this project is taken from Kaggle and is provided in CSV format. The training dataset contains 8,523 records and the test dataset contains 5,681 records.

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

# 5) Output Data Format:

• Predictions: CSV file containing the item identifiers, outlet identifiers, and the predicted sales.

• Plots/Tables:
    • Learning curves and feature importance plots saved as PNG files.
    • Regression performance metrics table displayed in the console and saved as a CSV file.

# 6) Parameters and Hyperparameters:

• Model Parameters:

    • n_estimators: Number of trees in the forest (Random Forest and XGBoost).
    
    • max_depth: The maximum depth of the trees.
    
    • min_samples_split: The minimum number of samples required to split an internal node (Random Forest).
    
    • min_samples_leaf: The minimum number of samples required to be at a leaf node (Random Forest).
    
    • learning_rate: Step size shrinkage used to prevent overfitting (XGBoost).
    
# 7) Hyperparameter Tuning:

    • RandomizedSearchCV is used to find the best parameters for the models based on a pre-defined grid of options.
    
# 8) Development Issues

    • Data Quality: Handling missing values and outliers in the data was challenging and required careful preprocessing to ensure accurate predictions.
    
    • Feature Selection: Determining which features were most predictive of sales involved extensive exploratory data analysis and testing various combinations in the models.
    
# 9) How to Use the Code?
    
    • Installation: Ensure that Python and necessary libraries (pandas, numpy, scikit-learn, xgboost, matplotlib) are installed.
    
    • Execution: Run the script from a command line or an IDE. Make sure the input data file path is correctly specified.
    
    • Output: Check the specified output directory for results and plots.


Clone the repository: git clone (https://github.com/AromaDsouza/BigMart_Sales_Prediction.git)


