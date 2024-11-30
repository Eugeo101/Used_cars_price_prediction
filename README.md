# Uber Fare Prediction 🚖💰  

This project focuses on predicting Uber ride fares based on ride attributes and location data using regression models.  

## 📝 Problem Statement  
Accurate fare prediction is crucial for optimizing customer satisfaction and operational efficiency. The goal is to predict Uber ride fares with high precision, leveraging feature engineering and machine learning techniques.  

## 🔍 Steps Followed  

### 1️⃣ Understanding the Data  
- Analyzed data columns and types.  
- Described numerical and categorical features for better understanding.  

### 2️⃣ Feature Engineering + Exploratory Data Analysis (EDA)  
- Engineered features like **Haversine Distance** to calculate the geographical distance between pickup and drop-off locations.  

- **Univariate Analysis:**  
  - Visualized value distributions using histograms and distplots.  
  - Explored categorical data with pie charts and count plots.  

- **Bivariate Analysis:**  
  - **Numerical vs Numerical:** Studied relationships using scatter and line plots.  
  - **Numerical vs Categorical:** Used box plots, violin plots, and strip plots for distribution analysis.  
  - **Categorical vs Categorical:** Compared data using bar plots and count plots.  

- **Multivariate Analysis:**  
  - Conducted pair plot analysis for feature relationships.  
  - Generated heatmaps to observe correlations.  

### 3️⃣ Pre-Processing  
- **Duplicate Handling:** Removed duplicate records for clean data.  
- **Train-Test Split:** Divided data into training and testing sets.  
- **Missing Values:** Detected and handled NaNs with imputation techniques.  
- **Outlier Detection:** Addressed outliers by setting valid ranges for latitude, longitude, and fare values.  
- **Encoding:**  
  - Applied **OrdinalEncoder** and **LabelEncoder** for ordinal data.  
  - Used **OneHotEncoder** and **BinaryEncoder** for nominal categories.  
- **Scaling:** Standardized features with **StandardScaler**, **MinMaxScaler**, and **RobustScaler**.  

### 4️⃣ Modeling  
- **Regression Models:**  
  - Experimented with **Linear Regression**, **Ridge**, **Lasso**, and **ElasticNet** models.  
- **Hyperparameter Tuning:**  
  - Used **GridSearchCV** and **RandomizedSearchCV** to optimize parameters.  
- **Validation:** Ensured models were neither underfitting nor overfitting.  
- **Performance Metrics:**  
  - **Validation Accuracy:** **82%**  
  - **Test Accuracy:** **81.1%**  
  - Model achieved a prediction confidence interval of ±3.7 from the estimated fare equation.  

### 5️⃣ Model Deployment  
- Saved the final tuned model for future prediction use.  
