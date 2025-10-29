# 🎧 Spotify Track Popularity Analysis

## 📘 Overview
This project explores **what makes a song popular on Spotify** using data-driven insights and machine learning.  
By analyzing a dataset of Spotify tracks, we investigate how various **audio features** — such as danceability, energy, loudness, and tempo — relate to a song’s **popularity**.

A **Random Forest Regressor** model is then trained to predict the popularity of a song based on its musical characteristics.

---

## 🎯 Objectives

- 🧹 Clean and prepare the Spotify dataset  
- 📊 Explore data trends and correlations among features  
- 🔥 Identify key factors influencing track popularity  
- 🤖 Build and evaluate a **Random Forest Regressor** model  
- 💡 Derive insights for predicting and improving track success  

---

## 📂 Dataset

- **Source:** Spotify Tracks Dataset (CSV format)  
- **Key Columns:**  
  `danceability`, `energy`, `loudness`, `tempo`, `acousticness`, `valence`, `speechiness`, `popularity`, etc.  
- **Target Variable:** `popularity` (0–100 scale)  

---

## 🧠 Machine Learning Workflow

### 1. Data Preprocessing
- Checked and removed missing values  
- Dropped irrelevant columns:  
  `Unnamed: 0`, `track_id`, `artists`, `album_name`, `track_name`, `track_genre`  

### 2. Exploratory Data Analysis (EDA)
- Distribution plots for **popularity**, **danceability**, etc.  
- Correlation heatmap to identify feature relationships  

### 3. Model Training
- **Algorithm:** Random Forest Regressor  
- **Train-Test Split:** 80% training / 20% testing  
- **Hyperparameters:** `n_estimators = 100`, `random_state = 42`  

### 4. Model Evaluation

| Metric | Score |
|---------|--------|
| Mean Squared Error (MSE) | 221.52 |
| R-squared (R²) | 0.55 |

✅ The model explains ~55% of the variance in song popularity, suggesting a moderate predictive capability.

---

## 📈 Key Insights

1. **Popularity Distribution:**  
   Most tracks fall into moderate popularity ranges; very few are extremely popular.  

2. **Feature Relationships:**  
   - **Energy** and **Loudness** are strongly correlated.  
   - **Acousticness** is negatively correlated with **Energy**.  
   - **Popularity** depends on multiple factors, not a single dominant feature.  

3. **Top Predictive Features:**  
   - Acousticness 🎸  
   - Tempo ⏱️  
   - Duration (ms) ⏳  
   - Danceability 💃  
   - Valence 😊  

4. **Feature Importance Visualization:**  
   The Random Forest model reveals that **acousticness, tempo, and duration_ms** are key drivers of popularity.

---

## 🚀 Future Improvements

- Try **advanced models** (e.g., XGBoost, Gradient Boosting, or Neural Networks)  
- Perform **hyperparameter tuning** to improve R²  
- Incorporate **external features** (artist followers, release date, genre trends)  
- Build an **interactive dashboard** using Streamlit or Plotly Dash  

---

## 🛠️ Technologies Used

| Category | Tools |
|-----------|--------|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Model | Random Forest Regressor |
| Environment | Google Colab / Jupyter Notebook |

---

## 📊 Example Visuals

- Popularity Distribution Histogram  
- Danceability Distribution Plot  
- Correlation Heatmap  
- Feature Importance Chart  

---

## 💬 Conclusion

* The Random Forest model can reasonably predict track popularity based on musical features.
* Popularity is **multi-dimensional**, influenced by audio properties and likely external factors (marketing, fan base, etc.).
* The project highlights the potential of **data analytics and ML** in understanding patterns behind hit songs.


