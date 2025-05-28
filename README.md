# 🔋 PowerPulse: Household Energy Usage Forecast

A machine learning project to forecast household power consumption using historical data. This project demonstrates EDA, feature engineering, model training, and evaluation using regression models.

---

## 📊 Project Objectives

- Predict household electricity usage using past data
- Analyze consumption patterns and key influencing factors
- Recommend strategies for energy optimization

---

## 🧱 Project Structure

| Folder/File               | Purpose                                  |
|--------------------------|------------------------------------------|
| `notebooks/`             | Jupyter Notebooks for EDA & Modeling     |
| `models/`                | Final saved ML model (MLPRegressor)      |
| `visuals/`               | Feature importance and other plots       |
| `README.md`              | Project summary and instructions         |
| `requirements.txt`       | Libraries needed to run the project      |

---

## 🛠️ Approach

1. Data loading and cleaning
2. Exploratory Data Analysis (EDA)
3. Feature engineering
4. Model training with 4 regressors
5. Hyperparameter tuning using GridSearchCV
6. Model evaluation using RMSE, MAE, R²
7. Model selection and export

---

## 📈 Results

| Model              | RMSE     | MAE      | R²       |
|-------------------|----------|----------|----------|
| **MLPRegressor**  | 0.0284   | 0.0174   | 0.9992   |
| Gradient Boosting | 0.0296   | 0.0182   | 0.9991   |
| Random Forest     | 0.0325   | 0.0192   | 0.9989   |
| Linear Regression | 0.0378   | 0.0242   | 0.9986   |

---

## 🔍 Key Insights

- Global intensity is the strongest predictor of active power.
- Usage peaks during 6–10 PM indicate evening load.
- Data smoothing via rolling averages improves model stability.

---

## 💾 How to Run

1. Clone the repo
2. Run notebooks in order from `/notebooks/`
3. Load and use the trained model from `/models/`

```bash
pip install -r requirements.txt
