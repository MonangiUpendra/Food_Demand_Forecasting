# 🍽️ Food Demand Forecasting using Machine Learning and Statistical Analysis

A predictive analytics project focused on accurately forecasting weekly food orders for a meal delivery company. Built with CatBoost, XGBoost, and advanced feature engineering, the model achieved over **80% prediction accuracy**.

---

## 📊 Problem Statement

Meal delivery companies face a critical challenge in managing inventory and reducing food wastage. The objective of this project is to predict the number of orders for each meal at a particular center for a given week using historical data.

---

## 📁 Dataset Overview

We used the following datasets:

- `train.csv` — Historical data with actual number of orders  
- `test.csv` — Input features without labels  
- `meal_info.csv` — Meal category and cuisine  
- `fulfilment_center_info.csv` — Center location, type, and operational area  

After merging and cleaning:

- `final_train.csv` → 456,548 rows × 15 columns  
- `final_test.csv` → 32,573 rows × 14 columns (excluding target)

---

## ⚙️ Technologies Used

- **Python**, **Pandas**, **NumPy**  
- **Scikit-Learn**, **CatBoost**, **XGBoost**  
- **Matplotlib**, **Seaborn** for EDA  
- **Google Colab**, **Jupyter Notebook**  
- **Streamlit** for deployment  

---

## 💠 Steps Followed

1. **Data Loading & Merging**  
2. **Feature Engineering**  
   - Price Difference, Discount Rate, Quarter  
   - Log transformation of target  
3. **Encoding Categorical Variables**  
4. **Model Training**  
   - Linear Regression  
   - Decision Tree Regressor  
   - Random Forest Regressor  
   - XGBoost Regressor  
   - ✨ **CatBoost Regressor (Best Performance)**  
5. **Model Evaluation** (MAE, RMSE, R², RMSLE)  
6. **Test Prediction & Submission File**  
7. **Web Interface Built with Streamlit**  

---

## ✅ Final Model Comparison

| Metric | CatBoost     | XGBoost |
|--------|--------------|---------|
| MAE    | 0.4185       | 0.4536  |
| RMSE   | 0.5354       | 0.5759  |
| RMSLE  | 0.1018       | 0.1085  |
| R²     | **0.8025**   | 0.7964  |

📌 **Final Model: CatBoost Regressor with 80.25% R² score**

---

## 📝 Project Highlights

- Achieved high accuracy without overfitting  
- Real-world feature engineering + log transformation  
- Built Streamlit app to showcase predictions interactively  
- Complete pipeline: data to model to UI  

---

## 🔮 Future Work

- Optimize hyperparameters using GridSearchCV  
- Automate data pipeline for real-time deployment  
- Integrate SQL dashboard for live reporting  

---

## 📂 How to Run

1. Upload data files in Colab / Jupyter  
2. Run `College_Project.ipynb`  
3. Launch app using `streamlit run app.py`  
4. Submit predictions using `submission.csv`

---

## 👤 Author

**Monangi Upendra**  
MCA Graduate | Python | ML | Android Firebase  
🔗 [LinkedIn](https://www.linkedin.com/in/monangi-upendra)  
🔗 [GitHub](https://github.com/monangiupendra)

---

## 📓 License

This project is for academic and learning purposes. All datasets are sourced from [Analytics Vidhya](https://datahack.analyticsvidhya.com/contest/food-demand-forecasting-challenge/).
