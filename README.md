## **Project description**

Project to analyze apartments sales data to gather incites about parameter affecting item price and how long it will take to sell it. Mentioned parameters later supposed to be used to build an automated system to track anomalies and fraudulent activity.

Project is made with **Python** and in **Jupyter Notebook** format.

<hr>

### **Main task**

Perform full exploratory data analysis, clear the data and check it for missing data or outliners. Identify most important features that affects apartment price and selling time. Visualize the data to support your finding and create a summary.

### **Data description**

For each apartment for sale, two types of data are available. The first are entered by the user, the second are obtained automatically based on map data.
All the data is presented in:

* **real_estate_data.csv** — full data about the apartments characteristics and sell price;

### **Project timeline:**
* EDA and data preprocessing was done.Initially separately for each data source and then processed data compiled for model training. Outliers removed, missing data handled.
* Joined data was checked for multicollinearity, scaled and some features were removed and some custom features added (**features engineering**)
* Five models were checked - **LinearRegression**, **Ridge**, **LightGBM**, **Catboost** and **RandomForestRegressor**
* For each model several hyperparameters were checked through **GridSearchCV**
* Prediction was done for each model with the best hyperparameters and all models compared via **MAE**.
* LightGBM was selected as the bst model and checked on test data
* **Best model MAE on test data was 6.18** and it is less than customer wanted so model was selected as appropriate.

<hr>
