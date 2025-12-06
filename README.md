# Used Car Price Prediction (CRISP-DM Project)

This project analyzes over 400,000 used car listings to identify what factors drive vehicle resale prices.  
Using the CRISP-DM framework, the workflow covers data understanding, cleaning, feature engineering, modeling,  
and delivery of insights for used car dealerships.

## 🚗 Project Overview
The goal is to build a machine learning model that predicts used car prices and reveals which vehicle attributes  
(year, mileage, manufacturer, condition, etc.) most influence resale value.

We tested multiple models and found that Random Forest provided the strongest predictive performance.

## ✅ Key Features
- Large-scale dataset with 400k+ used car listings.
- Extensive data cleaning + optimized preprocessing pipeline.
- Exploratory analysis of price vs. mileage, price vs. year, and category distributions.
- Multiple machine learning models with evaluation (Linear Regression, Ridge, ElasticNet, Random Forest).
- Log-transformed target for improved model stability.
- Feature importance extraction from the final Random Forest model.

## 📊 Best Model Result
| Model              | RMSE (lower is better) |
|-------------------|------------------------|
| Linear Regression | 7,285 |
| Ridge             | 7,291 |
| ElasticNet        | 7,262 |
| **Random Forest** | **5,417** |

Random Forest clearly outperformed all linear approaches.

## 🔍 Key Insights for Dealers
- Newer cars, low mileage, and good condition strongly increase resale value.
- Toyota, Honda, Subaru, and Lexus retain value exceptionally well.
- High-mileage and poor-condition vehicles sharply reduce price.
- The model helps guide trade‑in pricing, inventory purchases, and value‑based pricing strategy.

## 📁 Project Structure
```
├── data/                     # Raw or cleaned dataset (CSV not included in repo)
├── notebooks/                # Jupyter notebook containing full CRISP-DM workflow
├── plots/                    # All generated visualizations (PNG files)
├── README.md                 # Project documentation
└── requirements.txt          # Dependencies

```

## 🔧 Installation
```
pip install -r requirements.txt
```

## ▶️ Running the Project
Open the notebook:
```
jupyter notebook
```

Run each section sequentially (CRISP-DM aligned):
1. Business Understanding  
2. Data Understanding  
3. Data Preparation  
4. Modeling  
5. Evaluation  
6. Deployment  

## 🚀 Future Improvements
The following enhancements may be added later:
- Try **Gradient Boosting methods** (e.g., GradientBoostingRegressor, XGBoost, LightGBM).
- Hyperparameter tuning with Optuna or GridSearchCV.
- Save & deploy model using FastAPI or Streamlit.
- Create dashboard for interactive price predictions.
