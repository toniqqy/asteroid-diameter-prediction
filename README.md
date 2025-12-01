# Asteroid Diameter Prediction  
### Machine Learning • NASA JPL Dataset • Explainable AI (SHAP)

This project applies statistical machine learning to predict the diameter of asteroids using orbital, observational, and physical features from the NASA JPL Small-Body Database.  

It demonstrates skills in:
- Data cleaning & exploration  
- Correlation and scatterplot visualisation  
- Regression modelling (Linear, Decision Tree, Random Forest)  
- Model comparison using RMSE  
- Explainable AI using SHAP  
- Full notebook workflow and interpretation  

---

---

## Project Summary

The goal of this project is to predict an asteroid’s diameter (km) based on a set of 23 features, including:

- Orbital parameters (eccentricity `e`, semi-major axis `a`, inclination `i`, MOID, etc.)
- Observational metadata (`n_obs_used`, `data_arc`)
- Physical properties (`albedo`, `diameter_sigma`)

After exploring the data, non-linear patterns became clear, suggesting that tree-based models would perform better than linear methods.  

Three regression models were built:

1. Linear Regression (baseline)  
2. Decision Tree  
3. Random Forest (ensemble)  

The Random Forest achieved the best RMSE and was selected as the final model.

SHAP values were then used to interpret feature importance and the direction of their influence.

---

## Key Results

**Top predictors of asteroid diameter (via SHAP):**
- Lower albedo increases predicted diameter  
- Higher*number of observations slightly increases predictions  
- Orbital features such as eccentricity and MOID contribute smaller but meaningful adjustments  

**Model Performance:**
- Random Forest delivered the lowest RMSE, outperforming Linear Regression and Decision Trees  
- Ensemble methods captured complex non-linear relationships effectively  

---

## Visualisations Included

The notebook includes:

- Correlation heatmap (numeric-only)
- 5 scatter plots:
  - Diameter vs Albedo  
  - Diameter vs Number of Observations  
  - Diameter vs Eccentricity  
  - Albedo vs Eccentricity  
  - Diameter vs MOID  
- RMSE comparison table  
- SHAP summary plot  
- SHAP dependence plots for top features  

These visualisations illustrate both feature behaviour and model reasoning.

---

## Skills Demonstrated

### Machine Learning
- Model building (sklearn)  
- Hyperparameter awareness  
- Ensemble learning  
- Evaluation using RMSE  

### Data Analysis & Visualisation
- Exploratory data analysis (EDA)  
- Heatmaps, scatter plots  
- Detection of non-linear relationships  

### Explainable AI
- SHAP TreeExplainer  
- SHAP summary and dependence plots  
- Interpretation of feature influence  

### Tools & Technologies
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- SHAP  
- Google Colab  

---

## Why This Project Matters

This project shows the ability to:

- Work with real-world scientific datasets
- Build models that generalise well  
- Explain predictions using modern XAI methods  
- Present ML work in a clear, portfolio-friendly structure  

It’s a strong indicator of competencies in machine learning, data exploration, and model interpretability.

---

## 📎 Future Improvements

Potential next steps include:

- Random Forest hyperparameter tuning  
- Gradient Boosting and XGBoost models  
- Log-transforming diameter  
- Cross-validation  
- Additional feature engineering  

---

## About This Project

This work was completed as part of an applied machine learning unit and converted into a portfolio project to demonstrate practical ML and EDA skills using publicly available scientific data.

Feel free to explore the notebook or contact me for collaboration opportunities.

## Project Structure
📁 asteroid-diameter-prediction/  
├── CLR204_Asteroid_Diameter_Prediction.ipynb  
├── README.md  
└── /figures  
