# Loan approval prediction

## Objective
To predict *oan approval statu* based on applicants’ financial and demographic features.  

## Background
- When financial institutions evaluate loan applications, it is important to correctly assess an applicant’s ability to repay.  
- Using data such as income, credit score, employment type, and asset value, the project builds predictive models that help minimize default risks and improve decision-making.

## Dataset
Three separate public datasets were combined into one unified dataset for analysis:
- Dataset 1: 4269 records, contains applicant financial details
- Dataset 2: 615 records, loan application details
- Dataset 3: 5000 records, includes mortgage and asset information
- Final dataset: 9459 records and 13 features

## Data Preprocessing
- Unified column names across datasets (loan_status, income etc.)
- Combined 3 datasets into one DataFrame
- Removed duplicates and unnecessary variables
- Minor missing values imputed with mean values
- Major missing values imputed using MICE (Multiple Imputation by Chained Equations)
- Used IQR method to remove extreme outliers
- Final dataset after cleaning: 6917 records

## EDA
- Histograms for all numeric features  
- Boxplots for outlier detection  
- Density plots for comparing approved vs rejected loans  
- Heatmaps for overall and separate correlation analysis  

<img width="747" height="606" alt="Screenshot4" src="https://github.com/user-attachments/assets/d9ee5594-bbd9-468d-9cf6-0471d94c21dd" />


## Model
Implemented and compared four models:
- Decision Tree
- Random Forest
- K-Nearest Neighbors
- Logistic Regression

## Result

<img width="1332" height="250" alt="Screenshot5" src="https://github.com/user-attachments/assets/f7a800f5-8aa7-4f97-98c8-dbd144ea3874" />

Best model: Decision tree (Accuracy = 90.75%)

## Conclusion
- The Decision Tree model achieved the highest accuracy and interpretability.  
- Credit score, income, and loan amount were the most influential factors in loan approval decisions.  
- Logistic Regression performed worst, suggesting non-linear relationships among variables.  
- Cleaning and imputation using MICE significantly improved model performance and reproducibility.


