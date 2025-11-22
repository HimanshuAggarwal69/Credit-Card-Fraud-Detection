# Credit-Card-Fraud-Detection
Machine Learning project to detect fraudulent credit card transactions.

This project aims to detect fraudulent credit card transactions using various Machine Learning algorithms.  
The dataset is highly imbalanced, with only **492 fraud cases out of 284,807 transactions**, making this a real-world and challenging problem.

This project demonstrates end-to-end ML workflow including:
data preprocessing, EDA, handling imbalance (SMOTE), model building, evaluation, comparison, and final model selection.

---

# 📁 Dataset

The dataset used is the **Credit Card Fraud Detection Dataset** available on Kaggle.

- Total records: **284,807**
- Fraud cases: **492 (0.17%)**
- Legit transactions: **284,315**
- Features:  
  - PCA-transformed numerical features: **V1 to V28**  
  - Additional: **Time**, **Amount**  
  - Target: **Class (1 = Fraud, 0 = Not Fraud)**

> PCA transformation was used in the dataset to protect sensitive customer information.

---

# 🔍 Project Workflow

### ✅ 1. Exploratory Data Analysis (EDA)
- Checked dataset shape  
- Verified presence of class imbalance  
- Explored distribution of features  
- Understood PCA components (V1–V28)

### ✅ 2. Data Preprocessing
- Feature/Target separation (X, y)
- Train–test split (80/20)
- SMOTE used to balance training data

### ✅ 3. Machine Learning Models Used
The following models were trained and evaluated:

1. **Logistic Regression** (Baseline model)  
2. **Random Forest Classifier**  
3. **XGBoost Classifier** (Advanced gradient boosting)

---

# 📊 Model Performance Comparison

| Model               | Precision (Fraud) | Recall (Fraud) | F1 Score | ROC-AUC | Final Model |
|--------------------|-------------------|----------------|----------|---------|--------------|
| Logistic Regression | 0.12              | **0.91**       | 0.21     | **0.948** | No |
| Random Forest       | **0.83**          | 0.83           | **0.83** | 0.913   | ✔ **YES** |
| XGBoost             | 0.66             | 0.88           | 0.75     | 0.938   | No |

---

# 🏆 Final Model Selected: **Random Forest Classifier**

### ✔ Why this model?
- **Best Precision (0.83)** → Least false alarms  
- **Best F1-score (0.83)** → Balanced precision + recall  
- **Stable results** on imbalanced data  
- **Low false positives** and **low false negatives**  
- Performs well with PCA-transformed features

Random Forest provides the **best overall performance** for real-world fraud detection use cases.

---

# 📈 Visualizations

### 🔹 Confusion Matrix (Heatmap)
Shows true/false predictions visually.

### 🔹 ROC Curve  
AUC score: **0.913** for Random Forest.

### 🔹 Feature Importance (Random Forest)
Top contributing features:
- V14  
- V4  
- V10  
- V12  
- V17  

---

# 🧪 Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  
- XGBoost  

---

# 📝 How to Run This Project

1. Clone the repository:
  
2. Install dependencies:

3. Open the notebook and run all cells:


---

# 👨‍💻 Author

**Himanshu Aggarwal**

If you like this project, feel free to ⭐ the repo 😊

---

# 🧠 Future Improvements

- Add SHAP interpretability  
- Deploy model using Streamlit  
- Add API endpoint using FastAPI  
- Use neural networks for further comparison  

---

# ✔ Project Completed Successfully
This is a **resume-ready**, **industry-standard** ML project demonstrating:

- Full ML workflow  
- Handling imbalanced data  
- Evaluation with real metrics  
- Model comparison  
- Clean final model selection  




