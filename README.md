Melbourne House Price Prediction
1. Exploratory Data Analysis (EDA)
•	Explored the dataset using head(), tail(), shape, info(), describe(), and nunique(). 
•	Identified and handled missing values, removing records with missing target (Price) values. 
•	Examined feature distributions using histograms and detected potential outliers using boxplots. 
•	Generated a Pearson correlation heatmap for numeric features to identify potential multicollinearity. 

2. Data Preprocessing
•	Removed irrelevant and high-cardinality features such as Address and SellerG. 
•	Converted the Date column into datetime format and extracted Year and Month as predictive features before dropping the original Date column. 
•	Removed duplicate records. 
•	Applied one-hot encoding to categorical variables using pd.get_dummies(drop_first=True) to prepare the data for Linear Regression. 
•	Converted boolean features to integer format where required. 

3. Feature Engineering
•	Extracted Year and Month from the property sale date. 
•	Created dummy variables for categorical features using one-hot encoding. 
•	Separated the target variable (Price) from the predictor variables. 

4. Model Training & Evaluation
•	Split the dataset into training and testing sets. 
•	Trained a Linear Regression model as a baseline model. 
•	Evaluated performance using: 
o	R² Score 
o	Mean Absolute Error (MAE) 
o	Mean Squared Error (MSE) 
o	Root Mean Squared Error (RMSE) 
•	Visualized Actual vs Predicted Prices using a scatter plot. 

5. Feature Importance & Model Improvement
•	Trained a Random Forest Regressor to estimate feature importance. 
•	Removed low-importance feature groups and retrained the model to compare performance. 
•	Trained an XGBoost Regressor and compared its performance against Linear Regression. 
•	Achieved improved predictive performance using XGBoost. 

