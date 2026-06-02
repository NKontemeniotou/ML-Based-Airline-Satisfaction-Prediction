# ML-Based-Airline-Satisfaction-Prediction

# ✈️ Feature Selection & Model Performance Analysis (Airline Passenger Data)

This project explores how the number of selected features affects model performance using cross-validation scores. The goal is to identify the optimal subset of features that maximizes predictive performance while keeping the model efficient and interpretable.

---

## 📊 Objective

To evaluate how model performance changes as we incrementally add more features, and to determine the optimal feature set for prediction.

---

## 📈 Results Summary

The model was evaluated using cross-validation (CV). As more features were added, performance improved and eventually stabilized:

| Number of Features | Mean CV Score |
|--------------------|--------------|
| 1  | 0.7132 |
| 2  | 0.8048 |
| 3  | 0.9150 |
| 5  | 0.9348 |
| 10 | 0.9576 |
| 15 | 0.9591 |
| 20+ | ~0.9598 (plateau) |

📌 **Key Insight:**  
Model performance significantly improves up to ~10–15 features, after which it plateaus. This indicates diminishing returns from adding more features.

---

## 🧠 Selected Features

The final selected feature set includes:

- Flight Distance  
- Arrival Delay in Minutes  
- Inflight wifi service  
- Departure/Arrival time convenient  
- Ease of Online booking  
- Gate location  
- Food and drink  
- Online boarding  
- Seat comfort  
- Inflight entertainment  
- On-board service  
- Leg room service  
- Baggage handling  
- Check-in service  
- Inflight service  
- Cleanliness  
- Gender  
- Customer Type  
- Type of Travel  
- Class (encoded: Class_0, Class_1, Class_2)

---

## 🔍 Key Takeaways

- Feature selection improves both performance and efficiency
- Most predictive power is captured within the first ~10–15 features
- Additional features provide minimal improvement after saturation
- Strong importance of service quality and travel experience features in predictions

---

## 🛠️ Tools Used

- Python
- Scikit-learn
- Cross-validation (CV)
- Feature selection methods
- Pandas / NumPy

---

## 📌 Future Improvements

- Try different models (Random Forest, XGBoost, Logistic Regression comparison)
- Feature importance ranking (SHAP / permutation importance)
- Hyperparameter tuning for final model
- Deployment as a small prediction API

---

## 👤 Author

Data Analyst | Based in Cyprus  
Working at Rimes (Financial Data Operations)

---

⭐ If you find this useful, feel free to explore other projects in my GitHub portfolio.
