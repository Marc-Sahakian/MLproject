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
- **Deployment:** Local

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

- ✅ **Best Model:** Linear regression
- 📊 **R² Score (Test):** 0.88

---

## 🧱 Project Structure

student-performance-prediction/
│
├── app.py                        # Main Flask app for web deployment
├── setup.py                      # Package configuration
├── requirements.txt              # Python dependencies
├── README.md                     # Project documentation
│
├── templates/                    # HTML templates for the frontend
│   ├── index.html                # Landing page
│   └── home.html                 # Form for input and results display
│
├── src/
│   ├── components/               # Core ML modules: ingestion, transformation, training
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   │   └── model_evaluation.py
│   │
│   ├── pipeline/                 # Orchestrates training and prediction workflows
│   │   ├── train_pipeline.py
│   │   └── predict_pipeline.py
│   │
│   ├── utils.py                  # Helper functions
│   └── exception.py              # Custom exceptions
│
├── artifacts/                    # Stores trained model, preprocessor, and other outputs
├── logs/                         # Application and error logs
│
├── notebooks/                    # EDA and experimentation notebooks
│   └── eda.ipynb
