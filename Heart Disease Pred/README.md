![alt text](/ReadME_Files/MainImage_A1-9.jpg)

# Predicting Coronary Heart Disease Risk Using the Framingham Heart Study Dataset

High cholesterol is one of the leading risk factors for cardiovascular diseases, which are among the top health conditions affecting millions worldwide. To better understand the factors contributing to coronary heart disease (CHD) and predict its likelihood, I decided to analyze the Framingham Heart Study dataset. This dataset provides valuable insights into the relationships between various health and lifestyle factors, such as cholesterol levels, blood pressure, and smoking habits, and the onset of CHD. My objective was to determine if we could develop a reliable model to predict how likely an individual is to develop CHD, thus contributing to preventive healthcare efforts.

## The Dataset
[The Framingham Heart Study dataset](https://www.framinghamheartstudy.org/fhs-for-researchers/data-available-overview/) includes medical and demographic information collected from participants over a period of several years. It contains variables such as age, gender, cholesterol levels, blood pressure, smoking status, diabetes, and family history, among others. The dataset is widely used in health research to analyze cardiovascular risk factors and trends over time. In my project, I focused on identifying the most relevant predictors of CHD and applying machine learning algorithms to build a model capable of estimating an individual's risk of developing CHD within the next 10 years.

## Approach
### 1. [Exploratory Data Analysis (EDA)](https://github.com/VaishaliSharma19/springboard/blob/4f0ea29c6009443dadefc4d9b2397fdc20f91bb0/Heart%20Disease%20Pred/HeartDiseasePredictionData.ipynb):
I conducted EDA to understand the dataset, focusing on key variables like cholesterol, age, and blood pressure. I checked for correlations, missing values, and outliers, which helped guide the feature selection and ensure the data was ready for modeling.

### 2. [Data Visualization](https://github.com/VaishaliSharma19/springboard/blob/4f0ea29c6009443dadefc4d9b2397fdc20f91bb0/Heart%20Disease%20Pred/Framingham_Dataset_EDA.ipynb):
I used visualizations such as histograms, boxplots, and heatmaps to explore relationships between variables like cholesterol and CHD. These visuals highlighted important trends and patterns that influenced the model-building process.

### 3. [Data Preprocessing](https://github.com/VaishaliSharma19/springboard/blob/4f0ea29c6009443dadefc4d9b2397fdc20f91bb0/Heart%20Disease%20Pred/Pre-processing%20and%20Training%20Data%20Development_framingham_heart_disease.ipynb):
I handled missing data, normalized features, and encoded categorical variables. Afterward, I split the data into training and testing sets to prepare for model evaluation. This ensured the data was clean and ready for machine learning models.

### 4. [Modeling (Random Forest, XGBoost, Logistic Regression)](https://github.com/VaishaliSharma19/springboard/blob/4f0ea29c6009443dadefc4d9b2397fdc20f91bb0/Heart%20Disease%20Pred/Modeling_Frmingham_Dataset.ipynb):
I applied three models: Random Forest, XGBoost, and Logistic Regression. Random Forest was selected for its accuracy after hyperparameter tuning, while XGBoost added further precision. Logistic Regression served as a baseline model. Random Forest performed best, achieving the highest accuracy in predicting CHD risk.

## Results and Inference
The results show that Logistic Regression had moderate performance with balanced precision and recall, but its lower accuracy and ROC-AUC suggest it may not be the best choice for this dataset. In contrast, Random Forest delivered excellent performance across all metrics, with high accuracy, recall, precision, and F1 score, making it the most reliable model. XGBoost also performed well, closely matching Random Forest, though with slightly lower precision. Overall, Random Forest stands out as the best model due to its superior performance, while XGBoost remains a strong alternative, and Logistic Regression lags behind the ensemble methods.
