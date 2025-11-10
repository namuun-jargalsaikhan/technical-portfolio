#  Analysis and prediction of Apartment Prices in Ulaanbaatar, Mongolia

## Objective
To accurately predict apartment prices in Ulaanbaatar using various ML models and identify the key factors influencing housing prices.

## Background
- Ulaanbaatar’s real estate market is growing but still lacks transparency and open-access data.  
- Apartment price prediction is important for investors, buyers, and policymakers.  
- Few studies in Mongolia have combined web-scraped data with advanced model tuning.

## Data
- Source: Unegui.mn (https://www.unegui.mn) – Mongolia’s most widely used advertisement site
- Method: Web scraping using Python (Selenium, BeautifulSoup) 
- Final dataset: 19,400+ apartment listings, was collected on March 19, 2025  
- Target variable: Apartment price (₮, in millions)

## Data Preprocessing
- Removed duplicates or incomplete records  
- Converted object columns into numerical types
- Train-test split ratio: 80/20

## Model
Implemented and compared five models:  
- Linear Regression  
- Support Vector Regressor (SVR)  
- Random Forest Regressor  
- XGBoost  
- CatBoost

**Hyperparameter tuning methods**  
- GridSearchCV
- RandomizedSearchCV
- Bayesian Optimization

**Evaluation metrics** 
- R², RMSE, MAE, MSE

## Result
<img width="1205" height="281" alt="Screenshot" src="https://github.com/user-attachments/assets/e56aa363-04fe-4487-aa16-14b29e5aabd4" />

## Conclusion
- Around 10 % of listings were identified as undervalued, suggesting potential investment opportunities.  
- The analysis was limited to a single platform, and models were trained on asking prices rather than actual transactions.  
- Future work will integrate multiple data sources*and apply explainability techniques such as SHAP to improve model transparency.  
- Overall, ML models, especially Random Forest with Bayesian Optimization achieved high accuracy (R² = 0.973) in predicting apartment prices in Ulaanbaatar.  


