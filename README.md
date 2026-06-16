<div align="center">

# 🏠 House Price Prediction

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

> **Can we predict the price of a house from its features alone?**
> A regression project using Linear Regression — with real Kaggle data and measurable results.

</div>

---

## 📌 Problem Statement

Real estate pricing is complex — influenced by location, size, quality, age, and dozens of other factors. This project uses the **Kaggle House Prices dataset** to build a regression model that estimates residential property prices from numerical and categorical features, demonstrating a complete ML workflow from raw data to evaluation.

---

## 🎯 Project Highlights

| What | Detail |
|------|--------|
| 🧠 Algorithm | Linear Regression |
| 📦 Dataset | House Prices — Advanced Regression Techniques (Kaggle) |
| 🎯 Target | Sale Price (continuous value) |
| 📊 Key Features | Overall Quality, Living Area, Rooms, Year Built, and more |
| 📉 RMSE | 51,405.09 |
| 📈 R² Score | 0.655 (65.5% variance explained) |

---

## 🗂️ Project Structure

```
house-price-prediction/
│
├── house_price_prediction.ipynb  # Jupyter Notebook — full regression pipeline
├── requirements.txt              # Dependencies
├── images/                       # Visualization outputs
└── README.md
```

---

## 🔄 ML Pipeline

```
Load Data  →  EDA  →  Handle Missing Values  →  Feature Selection  →  Train Model  →  Evaluate
```

**Step-by-step:**

1. **Load Data** — Kaggle House Prices dataset
2. **EDA** — Explore features, distributions, correlations
3. **Handle Missing Values** — Drop or impute based on feature type
4. **Feature Selection** — Pick most relevant numerical and categorical features
5. **Train/Test Split** — Split for unbiased evaluation
6. **Train Model** — Linear Regression via Scikit-learn
7. **Evaluate** — RMSE and R² Score

---

## 📊 Key Findings

- 🏗️ **Overall Quality** is the single strongest predictor of sale price
- 📐 **Ground living area (GrLivArea)** has a strong positive linear relationship with price
- 📅 **Year Built** — newer houses consistently command higher prices
- 🚗 **Garage capacity** and **basement size** are significant secondary predictors

---

## 📈 Model Performance

| Metric | Score |
|--------|-------|
| RMSE | 51,405.09 |
| R² Score | 0.655 |

> The model explains ~65.5% of variance in house prices — a solid baseline for Linear Regression on this dataset.

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/keerthanad29/house-price-prediction.git
cd house-price-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook house_price_prediction.ipynb
```

> Dataset: Download from [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) and place in the project folder.

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

---

## 💡 What I Learned

- How to handle **real-world messy data** with many missing values
- Selecting features based on **correlation analysis**
- Understanding **RMSE vs R²** — what each metric actually tells you
- Why **Linear Regression** is a critical baseline before trying complex models

---

## 🔮 Future Improvements

- [ ] Try Random Forest / XGBoost for better accuracy
- [ ] Handle outliers more effectively
- [ ] Apply feature scaling and normalization
- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Deploy as a price estimator web app using Streamlit
