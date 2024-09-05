![alt text](/ReadME_Files/MainImage_A1-9.jpg)

# Predicting Coronary Heart Disease Risk Using the Framingham Heart Study Dataset

High cholesterol is one of the leading risk factors for cardiovascular diseases, which are among the top health conditions affecting millions worldwide. To better understand the factors contributing to coronary heart disease (CHD) and predict its likelihood, I decided to analyze the Framingham Heart Study dataset. This dataset provides valuable insights into the relationships between various health and lifestyle factors, such as cholesterol levels, blood pressure, and smoking habits, and the onset of CHD. My objective was to determine if we could develop a reliable model to predict how likely an individual is to develop CHD, thus contributing to preventive healthcare efforts.

## The Dataset
[The Framingham Heart Study dataset] (https://www.framinghamheartstudy.org/fhs-for-researchers/data-available-overview/) includes medical and demographic information collected from participants over a period of several years. It contains variables such as age, gender, cholesterol levels, blood pressure, smoking status, diabetes, and family history, among others. The dataset is widely used in health research to analyze cardiovascular risk factors and trends over time. In my project, I focused on identifying the most relevant predictors of CHD and applying machine learning algorithms to build a model capable of estimating an individual's risk of developing CHD within the next 10 years.

## Approach
### 1. Exploratory Data Analysis (EDA):
I conducted EDA to understand the dataset, focusing on key variables like cholesterol, age, and blood pressure. I checked for correlations, missing values, and outliers, which helped guide the feature selection and ensure the data was ready for modeling.

### 2. Data Visualization:
I used visualizations such as histograms, boxplots, and heatmaps to explore relationships between variables like cholesterol and CHD. These visuals highlighted important trends and patterns that influenced the model-building process.

### 3. Data Preprocessing:
I handled missing data, normalized features, and encoded categorical variables. Afterward, I split the data into training and testing sets to prepare for model evaluation. This ensured the data was clean and ready for machine learning models.

### 4. Modeling (Random Forest, XGBoost, Logistic Regression):
I applied three models: Random Forest, XGBoost, and Logistic Regression. Random Forest was selected for its accuracy after hyperparameter tuning, while XGBoost added further precision. Logistic Regression served as a baseline model. Random Forest performed best, achieving the highest accuracy in predicting CHD risk.

This approach effectively predicted CHD and provided valuable health insights.
