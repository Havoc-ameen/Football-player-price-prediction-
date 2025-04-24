

# ⚽ Football Player Market Value Prediction

This repository presents a machine learning project that predicts the **market value of football players** based on their skills and personal attributes. The model has been deployed using **Gradio**, allowing interactive predictions.

---

## 📌 Problem Statement

Football clubs often overpay or underpay for players due to inconsistent valuation methods. This project aims to solve that using a regression-based machine learning model to estimate the price of a player based on key attributes.

---

## 🔧 Technologies Used

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn**
- **Gradio**

---

## 💼 Use Case

Helps:
- Football agents with realistic player valuation  
- Clubs in transfer planning  
- Scouts to identify undervalued talent  

---

## 📁 Files in this Repo

| File                          | Description                                |
|-------------------------------|--------------------------------------------|
| `Football player price prediction.ipynb` | Complete ML workflow: EDA, preprocessing, training |  
| `requirements.txt`           | Python dependencies                        |
| `README.md`                  | Project overview                           |

---

## 📊 Exploratory Data Analysis (EDA)

We used data visualization to understand player attributes and their impact on market value.

### Key Insights:
- **Reactions** and **Ball Control** are top indicators of player value.
- **Age** shows a nonlinear relationship—very young or old players tend to have lower value.
- Market value distribution was skewed and log-transformed for better model performance.

---

## 📈 Model Development

Several regression models were trained and compared:
- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**

---

## ✅ Model Performance

| Model                  | R² Score | RMSE       |
|------------------------|----------|------------|
| Linear Regression      | 0.61     | 6.52       |
| Decision Tree Regressor| 0.74     | 4.87       |
| **Random Forest Regressor** | **0.81** | **4.21**     |

> **Random Forest Regressor** outperformed others in both accuracy and stability.

---

## 📌 Key Observations

- Models trained without feature scaling still performed well due to tree-based algorithms.
- Feature importance confirmed that:
  - **Reactions**, **Age**, and **Ball Control** were the most influential.
- Removing outliers improved the model’s RMSE significantly.
- The use of log transformation helped in stabilizing predictions for players with extremely high value.

---

## 🖥 Gradio App

Launch the Gradio app to test predictions in real time:

```bash
python
```
---

## 🎮 Sample Prediction

**Input**
- Age: 27  
- Reactions: 84  
- Ball Control: 88  
- Slide Tackle: 70  
- Stand Tackle: 75  

**Output**
- _Predicted Price_: 💰 **$42.3 Million**

---

## 🔮 Future Improvements

- Add league/club-level context  
- Scrape recent match data via API  
- Predict future market growth using time-series updates  




