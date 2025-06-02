# 🌦️ Weather Prediction Using Machine Learning

This project uses machine learning to predict the **next hour's weather condition** — classified as **Rainy**, **Cloudy**, or **Sunny** — based on current atmospheric data such as temperature, humidity, pressure, and more.

## 📌 Overview

The system processes real-time weather data, engineers relevant features, and applies a **Random Forest Classifier** to predict the next hour's weather condition. The model is trained and evaluated on labeled weather datasets, using a custom logic to derive labels from meteorological parameters.

## 🧠 Technologies Used

- Python 🐍
- Pandas & NumPy
- Scikit-learn
- Seaborn & Matplotlib
- Joblib (for model persistence)

## 📊 Features

- Classification of current weather as Rainy, Cloudy, or Sunny
- Predicts next hour's weather based on current readings
- Feature engineering using:
  - Time-based features
  - Rolling averages (3-hour)
  - Deltas in metrics like temperature and pressure
- Visualizations:
  - Boxplots for feature distribution
  - Correlation heatmaps
  - Confusion matrix
  - Feature importance chart

## 🧪 Model Evaluation

- **Model**: Random Forest Classifier (100 estimators)
- **Accuracy**: ~69.6%
- **Class Report**:
  - Rainy: Precision 0.57, Recall 0.54
  - Cloudy: Precision 0.52, Recall 0.12
  - Sunny: Precision 0.75, Recall 0.86

## 📁 Project Structure

```plaintext
├── weather_prediction.ipynb       # Main notebook with code and explanations
├── Weather data.xlsx              # Source dataset
├── hourly_weather_model.pkl       # Trained Random Forest model
├── hourly_weather_scaler.pkl      # Scaler for feature normalization
├── temp_by_weather.png            # Visualization: Temperature vs. Weather
├── humidity_by_weather.png        # Visualization: Humidity vs. Weather
├── cloud_by_weather.png           # Visualization: Cloud Cover vs. Weather
├── correlation_matrix.png         # Heatmap of feature correlations
├── confusion_matrix.png           # Model confusion matrix
├── feature_importance.png         # Top 15 feature importances
└── README.md                      # Project overview and documentation
