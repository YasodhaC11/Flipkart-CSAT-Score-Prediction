# 📞 Flipkart CSAT (Customer Satisfaction) Score Prediction

This project focuses on predicting the **Customer Satisfaction (CSAT) score** (1–5) based on agent performance, customer feedback, and support response details using Machine Learning and NLP techniques.

---

## 📌 Objective

The goal is to build a classification model that predicts CSAT scores from historical customer service data — helping identify unhappy customers and improve service quality.

---

## 🧰 Tech Stack & Tools

- **Languages & Libraries**: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
- **NLP Tools**: spaCy, TextBlob
- **Resampling Technique**: SMOTE (for handling class imbalance)
- **Model Evaluation**: Accuracy, F1-macro, Classification Report, Confusion Matrix
- **Model Tuning**: RandomizedSearchCV
- **ML Models**: Random Forest Classifier, XGBoost Classifier

---

## 🔍 Steps Involved

1. **Data Preprocessing**
   - Dropped irrelevant columns
   - Encoded categorical variables (Ordinal, Frequency, One-Hot Encoding)
   - Cleaned and lemmatized customer remarks using spaCy
   - Generated sentiment scores using TextBlob

2. **Feature Engineering**
   - Created features like agent frequency, response time, sentiment polarity
   - Handled rare categories in agent metadata
   - Converted datetime columns to numerical features

3. **Handling Imbalanced Data**
   - Used **SMOTE** to balance class distribution in the target (CSAT Score)

4. **Model Building & Evaluation**
   - Trained **Random Forest** and **XGBoost** classifiers
   - Tuned hyperparameters using **RandomizedSearchCV**
   - Evaluated with **Accuracy**, **Macro F1-Score**, and **Confusion Matrix**

---

## 📊 Results

| Model            | Accuracy | Mean F1-Macro (CV) |
|------------------|----------|--------------------|
| Random Forest    | 65.2%    | 26.1%              |
| XGBoost (Tuned)  | **70.8%**| **23.2%**          |

- XGBoost performed best in terms of accuracy
- However, **F1-Macro score revealed class imbalance impact**, as minority CSAT classes were harder to predict

---

## ✅ Key Learnings

- Accuracy alone is misleading for imbalanced multiclass problems
- Feature engineering from text (sentiment), agent metadata, and response timing is highly valuable
- SMOTE and proper evaluation metrics (like macro F1) are crucial for fair performance measurement

---

## 📁 Folder Structure

```bash
📦CSAT-Prediction
 ┣ 📜csat_model.ipynb
 ┣ 📜requirements.txt
 ┣ 📜README.md
 ┗ 📁data
    ┗ 📜csat_data.csv
