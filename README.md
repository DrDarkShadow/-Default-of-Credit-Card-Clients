# 💳 Credit Card Default Prediction

This project aims to predict whether a credit card client will default on their payment next month using a dataset of historical client data. The project covers a complete machine learning workflow from data preprocessing and feature engineering to model training, evaluation, and tuning.

---

## 📁 Dataset

- **Source:** UCI Machine Learning Repository  
- **Target Variable:** `default.payment.next.month` (0 = No default, 1 = Default)  
- **Attributes:** Client demographics, credit limit, past payments, bill statements, and payment behavior.

---

## 🔍 Workflow Overview

1. **Data Preprocessing**
   - Handled missing values
   - Removed/treated outliers using z-score and winsorization
   - Balanced the target classes using SMOTE

2. **Feature Engineering**
   - Created total bill, total payment, and average payment delay features
   - Addressed skewness using Yeo-Johnson transformation

3. **Feature Transformation**
   - Standardized numerical features using StandardScaler

4. **Dimensionality Reduction**
   - Applied PCA to reduce feature space while retaining 95% variance

5. **Model Building & Evaluation**
   - Trained and evaluated: Logistic Regression, Decision Tree, Random Forest, XGBoost, SVM
   - Compared performance using accuracy, precision, recall, F1-score, ROC-AUC

6. **Model Tuning**
   - Used GridSearchCV to fine-tune Random Forest parameters
   - Final model evaluated with confusion matrix and ROC curve

---

## 📊 Results

- Best Model: **Random Forest Classifier**
- Achieved highest F1-score and ROC-AUC
- Performance metrics tracked and compared using a summary table

---

## 📌 Key Takeaways

- Handled imbalanced classes with SMOTE
- Reduced dimensionality to prevent overfitting
- Optimized performance using Grid Search
- Full pipeline from EDA to deployment-ready model

---

## 🛠️ Tech Stack

- Python
- Scikit-learn
- XGBoost
- Pandas, NumPy, Matplotlib, Seaborn
- Imbalanced-learn
- Jupyter Notebook

---

## 📁 Project Structure

```
├── data/
│   └── Orignal_data.csv
├── Cleaned_data
├── Data_preprocessing
├── Exploratory_data_analysis
├── models/
│   └── best_model.pkl
├── credit_card_default_analysis.ipynb
├── README.md
└── requirements.txt
```

---

## ✅ How to Run

1. Clone the repo  
```bash
git clone https://github.com/yourusername/credit-card-default-prediction.git
cd credit-card-default-prediction
```

2. Install dependencies  
```bash
pip install -r requirements.txt
```

3. Run the notebook  
Open `credit_card_default_analysis.ipynb` and follow the steps.

---

## 📬 Contact

Created with ❤️ by **Prateek Gaur**  
📧 your.email@example.com  
🌐 [LinkedIn](https://linkedin.com/in/yourprofile)

---

## 📌 License

This project is licensed under the MIT License.
