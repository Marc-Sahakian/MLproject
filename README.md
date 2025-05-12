# 🎓 Student Performance Prediction

This project is an end-to-end machine learning pipeline designed to predict student exam scores based on personal and academic attributes. The solution includes data ingestion, preprocessing, model training with hyperparameter tuning, and deployment through a Flask-based web application.

---

## 📚 About the Project

The project aims to:
- Build a regression model to predict student scores
- Compare multiple ML models and select the best
- Deploy the solution in a web app for real-time predictions

---

## 🛠️ Tech Stack

- **Language:** Python
- **Web Framework:** Flask
- **ML Libraries:** scikit-learn, XGBoost, CatBoost, pandas, numpy
- **Model Persistence:** joblib
- **Frontend:** HTML, Jinja2 Templates
- **Deployment:** *[Replace with Render/Heroku/Local]*

---

## 🤖 Models Used

The following regression models were evaluated:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- CatBoost Regressor
- AdaBoost Regressor

Each model was tuned using a grid of hyperparameters. The model with the highest R² score on the test set was saved and deployed.

---

## 📈 Best Model Performance

- ✅ **Best Model:** *[Insert model, e.g., Random Forest Regressor]*  
- 📊 **R² Score (Test):** *[Insert score, e.g., 0.89]*  

---

## 🧱 Project Structure

