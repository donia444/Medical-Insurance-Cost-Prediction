# Medical-Insurance-Cost-Prediction
Predicting health insurance charges with Scikit-Learn. Improved model $R^2$ from 0.14 to 0.77 using data preprocessing and polynomial feature engineering."


# Medical Insurance Cost Prediction 🏥

## 📌 Project Overview
As part of my studies in **Computer Engineering**, I developed this project to predict individual medical costs. This model explores how demographic and lifestyle factors like **age, BMI, and smoking status** influence insurance charges.

## 📊 Key Results
I iterated through several models to find the best balance between accuracy and error margins:

| Model Version | R² Score | MAE (Error) | Status |
| :--- | :--- | :--- | :--- |
| Simple Linear (Age only) | 0.1452 | $8,986 | Baseline |
| Multiple Linear (Raw) | 0.7705 | $4,109 | Improved |
| **Polynomial Regression** | **0.7658** | **$4,259** | **Selected** |

*Note: While Polynomial Regression has a slightly higher MAE, it better captures the non-linear relationship between BMI and Smoking.*

---

## 🛠️ Data Handling & Engineering
To improve the model, I applied several engineering techniques:

1. **Categorical Encoding:** Converted 'Smoker' status into numerical data using `LabelEncoder`.
2. **Feature Scaling:** Applied `StandardScaler` to Age and BMI so the model treats them with equal importance.
3. **Polynomial Features:** Added $BMI^2$ to capture the "upward curve" in costs for high-BMI individuals.
4. **Outlier Analysis:** Used the **IQR Method** to identify extreme charges and experimented with **Log Transformations** to normalize the target distribution.



---

