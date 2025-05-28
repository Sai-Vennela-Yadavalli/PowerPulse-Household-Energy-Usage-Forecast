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

Our goal was to forecast household energy consumption using historical data. We followed a structured Data Science pipeline:

1. **Data Loading & Preprocessing**
   - Combined date and time into a single datetime column
   - Handled missing values
   - Converted all numerical features to appropriate types

2. **Exploratory Data Analysis (EDA)**
   - Analyzed energy usage patterns using histograms, trend lines, and correlation heatmaps
   - Detected outliers using the IQR method

3. **Feature Engineering**
   - Created daily average, 60-minute rolling average, and peak hour flags
   - Normalized numerical features for improved model performance

4. **Model Selection and Training**
   - Trained multiple regression models: Linear Regression, Random Forest, Gradient Boosting, and MLPRegressor
   - Used GridSearchCV for hyperparameter tuning on top models

5. **Model Evaluation**
   - Evaluated each model using RMSE, MAE, and R²
   - Selected MLPRegressor as the best-performing model

6. **Model Saving**
   - Saved the trained model using `joblib` for future use or deployment

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

bash
pip install -r requirements.txt


**## 🔗 Connect With Me**
If you found this project interesting or would like to collaborate, feel free to connect with me on LinkedIn:

👉 [Sai Vennela Yadavalli](https://www.linkedin.com/in/sai-vennela-yadavalli-8b854432a)

I'd love to hear your feedback or discuss more about Data Science and Machine Learning!

