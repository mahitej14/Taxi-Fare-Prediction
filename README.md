# 🚕 Taxi Fare Prediction Using Machine Learning

## 📌 Project Overview

This project uses Machine Learning regression algorithms to predict the total taxi fare based on trip details such as passenger count, trip distance, and pickup time.

The project is implemented in Python using Google Colab or Jupyter Notebook. It covers data preprocessing, feature engineering, model training, evaluation, hyperparameter tuning, and predictions for new trips.

## 🎯 Objectives

- Clean and analyze taxi trip data.
- Select relevant features for fare prediction.
- Train and compare multiple regression models.
- Evaluate models using standard regression metrics.
- Tune model hyperparameters.
- Predict the estimated total amount for a new taxi trip.

## 📂 Dataset

**Dataset name:** Revenue for Cab Drivers

**Source:** Kaggle

**Dataset link:** https://www.kaggle.com/datasets/diishasiing/revenue-for-cab-drivers

The dataset contains taxi-trip information used for data analysis and Machine Learning.

Please refer to the original Kaggle page for the dataset description, files, and licensing terms.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost (optional)
- Google Colab

## ⚙️ Project Workflow

1. Load the taxi dataset.
2. Clean the data and handle missing values.
3. Extract pickup hour, day, and month.
4. Select input features and the target variable.
5. Split data into training and testing sets.
6. Train multiple regression models.
7. Evaluate model performance.
8. Tune model hyperparameters.
9. Predict the total taxi amount for new trip details.

## 📊 Input Features

The model uses these five input features:

| Feature | Description |
|---|---|
| `passenger_count` | Number of passengers |
| `trip_distance` | Estimated trip distance in miles |
| `pickup_hour` | Pickup hour (0–23) |
| `pickup_day` | Day of the week (0–6) |
| `pickup_month` | Pickup month (1–12) |

**Target variable:** `total_amount`

Fare components such as `fare_amount`, `tip_amount`, tolls, and surcharges are excluded from the input features to avoid target leakage when predicting the total amount.

## 🤖 Machine Learning Models

The notebook compares regression models, including:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Support Vector Regression (SVR)
- K-Nearest Neighbors (KNN)
- Decision Tree Regressor
- Random Forest Regressor
- AdaBoost Regressor
- Gradient Boosting Regressor
- XGBoost Regressor (if available)

The final model is selected through the model evaluation and tuning process in the notebook.

## 📈 Evaluation Metrics

The project uses the following regression metrics:

- **MAE:** Mean Absolute Error
- **MSE:** Mean Squared Error
- **RMSE:** Root Mean Squared Error
- **R² Score:** Coefficient of determination

The notebook also includes model comparisons and diagnostic plots.

## 🚀 How to Run the Project

### Using Google Colab

1. Clone or download this GitHub repository.
2. Open `taxi_fare_prediction.ipynb` in [Google Colab](https://colab.research.google.com/).
3. Download the dataset from the Kaggle link above.
4. Upload the dataset to Colab if it is not already available.
5. Ensure the dataset filename and notebook file path match.
6. Run all notebook cells from top to bottom.
7. Review the model evaluation results and try the prediction section.

### Run Locally

Install the required packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

Clone the repository:

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `taxi_fare_prediction.ipynb` and run the cells in order.

## 🔮 Example Prediction

The notebook prompts the user to enter:

- Number of passengers
- Estimated trip distance
- Pickup hour
- Pickup day of the week
- Pickup month

It then displays the estimated total taxi amount.

The prediction is an estimate and is not a guarantee of the actual fare.

## 📁 Repository Structure

Taxi-Fare-Prediction/
├── README.md
└── taxi_fare_prediction.ipynb

The dataset can be downloaded separately from Kaggle rather than committed to GitHub.

## 🔐 Dataset and File Notes

- Credit the original dataset creator and include the Kaggle link.
- Check the dataset license and redistribution terms before committing the dataset file.
- If the dataset is large, keep it on Kaggle and link to it from this README instead.
- Do not commit credentials, API tokens, or private information.

## 🌱 Future Improvements

- Train models using more of the available dataset.
- Improve feature engineering and data quality.
- Evaluate predictions on unseen data.
- Explore route-based distance estimates.
- Build a simple web application for fare prediction.

## 👤 Author

**Mahitej Naroju**

Profile link: https://github.com/mahitej14

## 📄 License

The notebook code and the third-party dataset may have different licensing terms. Add an appropriate license for your own code, and follow the original dataset's license for data use and redistribution.

---

*This project was developed for educational purposes to demonstrate a Machine Learning regression workflow.*
