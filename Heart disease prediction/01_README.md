# Heart disease prediction

## Objective
To analyze clinical data of patients to predict heart disease using ML techniques.

## Background
- Heart disease is one of the most common causes of death worldwide.
- Through visualization of patient data, I aimed to identify meaningful patterns and relationships between health indicators such as age, cholesterol, and ECG results.

## Dataset
- Source: Public heart disease dataset from kaggle https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction 
- Total samples: 918 patients  
- Target variable: HeartDisease

## Data preprocessing
- Verified no missing or duplicated records  
- Converted object columns into numerical types 
- Standardized numerical features  
- Train-test split ratio: 80/20

## Data Visualization
Visualization methods:
- Histograms for age, cholesterol, and blood pressure  
- Category frequency plots for gender, ECG, and chest pain type  
- Pairplots to explore relationships between multiple features  
- Correlation heatmap to understand relationships among variables  
- Color decision tree visualization for model interpretability

Pairplot for example:
<img width="913" height="866" alt="Screenshot1" src="https://github.com/user-attachments/assets/ba6943c5-7bf6-496a-aca1-bc09e9648b39" />

## Model
Implemented and compared six models:
- Decision Tree  
- Random Forest  
- Logistic Regression  
- Gradient Boosting  
- K-Nearest Neighbors  
- Naive Bayes  

## Result 
<img width="1282" height="321" alt="Screenshot2" src="https://github.com/user-attachments/assets/6608c4c8-454a-465e-bd4f-4de2a423b73e" />

Best performing model: Gradient Boosting (Accuracy 0.842, F1 0.856)

## Color decision tree Visualization
- An explainable decision tree visualization was created to highlight important variables and simplify rules for classification.  
- By separating the model into Type 1 and Type 2 structures and removing unnecessary conditions, the rules became easier to interpret.

Output:
<img width="1497" height="568" alt="Screenshot3" src="https://github.com/user-attachments/assets/79f669b8-f63b-4ca9-9289-1dc22c2c4ea8" />

## Conclusion
- The Gradient Boosting model showed the highest prediction performance.
- Visualization identified ST_Slope as the most influential variable for detecting heart disease.
- This project combines visual analytics with interpretable modeling.
- The models were trained on data from 918 patients, and it is expected that collecting and training on a larger dataset would lead to even better model performance.
