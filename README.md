# Amazon-Product-Reviews-Sentiment-Analysis-NLP.
Project Overview
This project involves analyzing sentiment from Amazon product reviews, specifically in the electronics sector. 
We processed raw review data to identify key sentiments (positive, negative, and neutral) and used machine learning models to predict overall product ratings based on review texts. 
The goal is to derive actionable insights for businesses to understand customer feedback better and optimize their products and services.

Key Features
Sentiment Classification: Predicts sentiments (positive, negative, neutral) from Amazon reviews using machine learning models.
Machine Learning Models: Logistic Regression, Support Vector Machine (SVM), Decision Tree, and Random Forest were evaluated.
Best Model: Random Forest provided the most robust performance, especially after cross-validation.
Data Visualization: Word clouds, histograms, and time-series visualizations were used for a better understanding of data distribution and sentiment trends.
Steps Involved
1. Data Exploration
Initial examination of the dataset to understand its structure.
Summary statistics and visualizations to understand the distribution of review ratings and sentiments.
2. Data Cleaning & Preprocessing
Text Preprocessing: Lowercasing, removing punctuation, stopwords, and non-alphanumeric characters.
Feature Engineering: Created features from the review text, including sentiment polarity and time-based features like year and month from review timestamps.
3. Exploratory Data Analysis (EDA)
Visualizations: Word clouds to represent frequent terms in reviews, bar plots for sentiment distribution, and time-series plots to observe review trends over time.
4. Sentiment Analysis Models
Logistic Regression: Used for binary classification of sentiments.
Support Vector Machine (SVM): Identified sentiment classes with a higher degree of separation in feature space.
Decision Tree: Captured non-linear relationships but struggled with overfitting.
Random Forest: Performed the best in terms of accuracy and handling noisy data, especially after cross-validation.
5. Model Evaluation
Metrics Used: Accuracy, precision, recall, and F1-score for each model.
Cross-validation: 5-fold cross-validation was applied to ensure models generalize well to unseen data.
Random Forest: Achieved an accuracy of 74% with balanced precision and recall, making it the best-performing model.
Tools & Technologies
Programming Language: Python
Libraries:
NLTK: Text preprocessing and sentiment analysis.
Pandas: Data manipulation and analysis.
Scikit-learn: Machine learning model development and evaluation.
Matplotlib & Seaborn: Data visualization.
SMOTE: Balancing the dataset through synthetic oversampling.
Results
Best Model: Random Forest achieved the highest accuracy (74%) and balanced performance across sentiment classes.
Insights: Positive sentiments were more frequent in the dataset. Negative sentiments were harder to classify, but Random Forest handled this challenge better than other models.
Visualization Impact: Helped in identifying trends, common words, and customer concerns within the dataset.
Conclusion
This project demonstrates the application of machine learning to extract actionable insights from customer reviews. The Random Forest model proved most effective in sentiment analysis, providing balanced performance across sentiment categories. These findings can help businesses make data-driven decisions, improve customer satisfaction, and strategize their offerings.
