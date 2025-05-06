# 🧪 Pharmaceutical Sales Prediction Across Multiple Stores

A machine learning project to forecast pharmaceutical sales across multiple stores using historical data, with the aim of optimizing supply chain decisions and improving revenue planning.

---

## 📌 Problem Statement

Pharmaceutical companies and distributors need to accurately forecast sales at various retail locations to ensure optimal inventory, reduce losses, and meet demand efficiently. This project aims to predict future sales volumes using historical sales and store-level information.

---

## 🎯 Objectives

- Build a robust machine learning model to predict pharmaceutical sales per store.
- Minimize inventory issues and overstocking.
- Provide actionable insights into sales trends across regions.
- Enable data-driven supply chain and operational decisions.

---

## 📥 Data Collection

- **Source**: [Add source - e.g., Kaggle or internal company data]
- **Type**: Structured
- **Size**: [Number of rows and columns]
- **Features**: Store ID, Product Type, Sales Volume, Promotion Status, Date, Region, etc.

---

## 🧹 Data Preprocessing

- Handled missing values.
- Encoded categorical variables using Label and One-hot encoding.
- Normalized features using StandardScaler.
- Removed outliers using IQR method.
- Split data into training and testing sets (e.g., 80/20).

---

## 📊 Exploratory Data Analysis (EDA)

- Analyzed sales distribution across stores and regions.
- Identified top-selling product categories.
- Visualized correlation between promotions and sales.
- Heatmaps, histograms, boxplots, and line plots used for insights.

---

## 🛠️ Feature Engineering

- Created time-based features (e.g., month, quarter).
- Generated lag features for previous sales.
- Applied dimensionality reduction (PCA) to reduce noise.

---

## 🧠 Model Selection

Evaluated multiple models:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor
- LightGBM
- Neural Networks (MLP)

---

## 🏋️ Model Training

- Applied K-Fold Cross Validation for robust performance check.
- Used GridSearchCV and RandomizedSearchCV for hyperparameter tuning.
- Selected best-performing model based on validation metrics.

---

## 📈 Model Evaluation

- **Best Model**: [Model name, e.g., XGBoost]
- **Metrics Used**:
  - R² Score
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
- Performance comparison done across all models.

---

## 🚀 Model Deployment (Optional)

Deployed the best model using:

- **Frontend**: Streamlit
- **Backend**: FastAPI (for scalable REST API)
- **Hosting**: Render / Heroku / AWS

---

## 🧾 Conclusion

- Best model achieved R² of **XX%** on test data.
- Significant improvement over baseline models.
- Insights from model helped understand sales patterns and influence of promotions.

---

## 🔭 Future Work

- Incorporate external data: holidays, weather, regional events.
- Use advanced time series models (LSTM, Prophet).
- Automate retraining and deployment with MLOps pipeline.
- Real-time prediction and dashboards.

---

## 🗂️ Project Structure

```bash
pharma-sales-prediction/
│
├── data/                # Raw and cleaned datasets
├── notebooks/           # EDA and modeling notebooks
├── models/              # Trained and serialized model files (.pkl, .joblib)
├── app/                 # Deployment code (Streamlit/FastAPI)
├── utils/               # Helper scripts and feature engineering
├── README.md            # Project overview
├── requirements.txt     # Python dependencies
└── LICENSE              # License file (MIT or others)
