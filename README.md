
🌤️ Weather Forecasting ML

A complete machine learning pipeline for predicting temperature & precipitation using synthetic weather data.

📘 Project Overview

This project demonstrates a full end-to-end machine learning workflow for weather forecasting.
It includes:
	•	Data generation (synthetic weather dataset)
	•	Data preprocessing and visualization
	•	Model training (Random Forest Regressor)
	•	Saving/loading ML models with joblib
	•	A clean and modular project structure
	•	Jupyter Notebook analysis

📂 Project Structure

weather-forecasting-ml/
│── data/                  # data storage (empty tracked using .gitkeep)
│── models/                # trained ML models
│   └── weather_model.pkl
│── notebooks/
│   └── weather_forecast_analysis.ipynb
│── src/
│   └── (future Python scripts here)
│── requirements.txt
│── README.md
│── .gitignore

🧠 Modeling Approach

Algorithm Used
	•	RandomForestRegressor
	•	Handles non-linear relationships
	•	Works well with noisy or synthetic data
	•	Minimal preprocessing required

Target Variables

The model predicts:

Feature                 Meaning
temperature             Next-day temperature
precipitation           Rainfall mm

📊 Visuals (Plots Used in the Notebook)

1️⃣ Pairplot (Feature Relationships)
sns.pairplot(df)
2️⃣ Actual vs Predicted Temperature
plt.scatter(y_test, y_pred)
plt.xlabel("Actual Temperature")
plt.ylabel("Predicted Temperature")
3️⃣ Feature Importance
model.feature_importances_

🛠️ Technologies Used
	•	Python 3.9+
	•	Pandas
	•	NumPy
	•	Scikit-Learn
	•	Matplotlib
	•	Seaborn
	•	Joblib

📈 Model Performance

Metric          Value
MAE             ~1.2
R²Score         ~0.88
RMSE            ~1.6

(Exact values depend on seed + synthetic randomness)