# 🚦 Flipkart Gridlock Hackathon 2.0 — Traffic Demand Prediction

An advanced Machine Learning solution developed for the **Flipkart Gridlock Hackathon 2.0**, focused on predicting real-time traffic demand using road infrastructure, weather conditions, vehicle flow, and temporal traffic patterns.

This project leverages **CatBoost Regressor** along with feature engineering techniques to build a high-performance traffic forecasting pipeline.

---

# 🔥 Problem Statement

Predict the **traffic demand** of a location using:

* Road information
* Weather conditions
* Traffic infrastructure
* Temporal patterns
* Vehicle movement indicators

The challenge involved building a regression model capable of understanding real-world traffic behavior patterns.

---

# 🚀 Achievements

✅ Built complete ML pipeline from scratch
✅ Applied timestamp-based feature engineering
✅ Used CatBoost for categorical feature handling
✅ Achieved **87.84+ online score** on leaderboard
✅ Generated competition-ready submission pipeline

---

# 📊 Dataset Features

| Feature       | Description                 |
| ------------- | --------------------------- |
| geohash       | Encoded geographic location |
| day           | Day identifier              |
| timestamp     | Traffic timing data         |
| RoadType      | Type of road                |
| NumberofLanes | Number of lanes             |
| LargeVehicles | Presence of heavy vehicles  |
| Landmarks     | Nearby landmarks            |
| Temperature   | Temperature data            |
| Weather       | Weather conditions          |
| demand        | Target traffic demand       |

---

# 🧠 Machine Learning Pipeline

```text
Data Collection
      ↓
Data Cleaning
      ↓
Timestamp Processing
      ↓
Feature Engineering
      ↓
Categorical Feature Handling
      ↓
Train-Test Split
      ↓
CatBoost Regression
      ↓
Prediction Generation
      ↓
submission.csv
```

---

# ⚙️ Feature Engineering

Key engineered features:

* Hour extraction from timestamp
* Minute extraction
* Peak hour detection
* Temporal traffic behavior analysis

Example:

```python
df['hour'] = df['timestamp'].dt.hour
df['minute'] = df['timestamp'].dt.minute
```

---

# 🌳 Model Used

## CatBoost Regressor

Why CatBoost?

* Handles categorical data efficiently
* Minimal preprocessing required
* Strong performance on tabular datasets
* Excellent regression capabilities

---

# 📈 Evaluation Metric

Model performance was evaluated using:

R^2 = 1 - \frac{\sum (y_i - \hat{y}_i)^2}{\sum (y_i - \bar{y})^2}

Where:

* ( y_i ) → Actual values
* ( \hat{y}_i ) → Predicted values

---

# 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Scikit-Learn
* CatBoost
* Jupyter Notebook

---

# 📂 Project Structure

```text
├── train.csv
├── test.csv
├── submission.csv
├── flipkart.ipynb
├── README.md
```

---

# 🚀 How to Run

## Install Dependencies

```bash
pip install pandas numpy scikit-learn catboost
```

---

## Run Notebook

```bash
jupyter notebook
```

Open:

```text
flipkart.ipynb
```

---

# 📤 Output

The final model generates:

```text
submission.csv
```

Format:

| Index | demand |
| ----- | ------ |
| 1     | 52.3   |
| 2     | 61.8   |

---

# 🔍 Interesting Observation

During leaderboard evaluation, a large number of participants achieved near-perfect scores (~100 R²), raising interesting discussions around:

* Data leakage possibilities
* Public leaderboard overfitting
* Extremely predictable traffic patterns
* Hidden evaluation differences

---

# 🎯 Applications

* Smart Traffic Systems
* Urban Mobility Analytics
* Congestion Prediction
* Intelligent Transportation
* Smart City Infrastructure

---

# 👨‍💻 Author

HARSH GUPTA 🚀

---

# ⭐ If you found this project interesting, consider starring the repository!


# FLIPKART-GRIDLOCK-HACKATHON-2026-
An advanced Machine Learning solution developed for the Flipkart Gridlock Hackathon 2.0, focused on predicting real-time traffic demand using road infrastructure, weather conditions, vehicle flow, and temporal traffic patterns.
