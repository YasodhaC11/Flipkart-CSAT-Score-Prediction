# Flipkart-CSAT-Score-Prediction

Project Objective
To identify key drivers of customer satisfaction and predict CSAT (Customer Satisfaction) scores based on customer feedback using NLP and machine learning. The goal is to support Flipkart in enhancing customer service strategies and improving overall satisfaction.

🧰 Technologies Used
Python,Pandas, NumPy
Scikit-learn
XGBoost
Matplotlib, Seaborn

📁 Dataset
Customer reviews, CSAT scores, and other related data.

🧹 Data Preprocessing
Removed nulls, duplicates, and irrelevant fields

📈 Exploratory Data Analysis
Word frequency distribution in positive/negative reviews
Distribution of CSAT scores
CSAT trends across shifts, product types

📊 Hypothesis Testing
Hypothesis:
Is there a significant difference in CSAT scores across agent shifts?
Test Used: One-way ANOVA

🤖 Models Built
Logistic Regression
Random Forest
✅ XGBoost (Final Model - Best Accuracy)

Final Evaluation Metrics:
Accuracy: ~71%
Precision, Recall, F1-Score used due to class imbalance

💡 Key Insights
High-CSAT reviews mention delivery speed and product quality
Low-CSAT reviews highlight delays, damaged items, and unresolved issues

🚀 Future Enhancements
Hyperparameter tuning (GridSearchCV)
Deep learning models (LSTM/BERT)
Real-time CSAT prediction integration

