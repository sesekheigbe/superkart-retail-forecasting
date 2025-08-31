# superkart-retail-forecasting

## Executive Summary
This project developed a machine learning pipeline to forecast store revenue for SuperKart.  
Through exploratory data analysis, feature engineering, and model comparisons, Random Forest was chosen over XGBoost for its efficiency and comparable performance.  
The solution was deployed with a Flask backend and Streamlit frontend on Hugging Face Spaces, demonstrating an end-to-end approach that connects data science outputs to business revenue impact.

---

## Project Overview
Retailers face challenges predicting future demand due to seasonality, promotions, and customer behavior.  
This project applies regression and ensemble tree-based models (Random Forest, XGBoost) to predict store revenue and demonstrates full-stack ML deployment.

---

## Key Steps
- Exploratory Data Analysis (EDA): Identified sales patterns, seasonal trends, and correlations.  
- Feature Engineering: Created lag features, encoded categorical variables, added holiday/promotion indicators.  
- Model Training: Compared Linear Regression, Random Forest, and XGBoost.  
- Model Selection: Evaluated trade-offs between Random Forest and XGBoost to balance performance vs. complexity.  
- Backend Development: Built a Flask API to serve model predictions.  
- Frontend Development: Developed a Streamlit UI for interactive forecasting.  
- Deployment: Integrated backend and frontend and deployed the complete app on Hugging Face Spaces.  

---

## Results
- Both Random Forest and XGBoost achieved similar performance  
  (R² = 0.668, Adjusted R² = 0.667, MAPE = 0.187).  
- Random Forest was selected as the final model since XGBoost required more setup and tuning without additional benefit.  

### Business Impact
Improved demand forecasting enables smarter inventory and stock management decisions, reducing costs from overstock/stock-outs and ultimately driving higher revenue and profitability.  

---

## Key Learnings
- Built an end-to-end ML pipeline (EDA → Feature Engineering → Modeling → Deployment).  
- Compared Random Forest and XGBoost, learning to evaluate trade-offs when models deliver similar performance.  
- Gained experience deploying a Flask API (backend) with a Streamlit UI (frontend) on Hugging Face Spaces.  
- Learned how ML outputs connect to business outcomes by linking demand forecasts to inventory optimization and revenue impact.  

---

## Project Architecture

```mermaid
flowchart LR
    A[Data Input] --> B[Feature Engineering]
    B --> C[ML Model (RF, XGBoost)]
    C --> D[Flask API (Backend)]
    D --> E[Streamlit UI (Frontend)]
    E --> F[Hugging Face Spaces Deployment]



---

## Project Structure
superkart-store-revenue-prediction/
 ├── SuperKart_Forecasting.ipynb   # Main notebook
 ├── requirements.txt              # Dependencies
 └── README.md                     # Project documentation

👤 Author: Solomon O. Esekheigbe  
🔗 GitHub: [sesekheigbe](https://github.com/sesekheigbe)
