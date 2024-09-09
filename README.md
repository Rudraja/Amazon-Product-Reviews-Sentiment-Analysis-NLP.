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

6. Model Evaluation
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

Results:

Without Cross Validation:
Logistic Regression: The accuracy of the logistic regression model is about 70%. It shows balanced performance with constant precision, recall, and F1-score in all three sentiment classes. In contrast to good sentiments, it has a little trouble categorising negative sentiments.
Linear SVM: With an accuracy of roughly 71%, the linear support vector machine (SVM) model performs better than logistic regression. It performs better in terms of recall and precision when classifying both positive and negative emotions, although it excels most at classifying pleasant emotions. This demonstrates how well the model can divide sentiment classes inside the feature space.
Decision Tree: The accuracy of the decision tree model is approximately 68%. Its accuracy and recall for neutral thoughts are reasonable, but when it comes to negative sentiments, it performs poorly overall. The models inferior performance could be attributed to overfitting, as evidenced by the differences in recall and precision scores across sentiment classes.
Random Forest: The accuracy of the random forest model is about 69%. Robust performance is demonstrated by the balanced precision, recall, and F1-score across emotion classes. But just like the decision tree model, it has trouble categorizing negative emotions, which lowers the precision 17 score for this class. Despite this, compared to individual decision trees, the random forest model performs better overall due to its ensemble aspect, which helps reduce overfitting.

With Cross Validation:
Logistic Regression: The logistic regression model performs well in sentiment classification, with an accuracy of 0.70 and a mean cross-validation score of about 0.70. It consistently demonstrates a capacity to categories sentiments by maintaining balanced precision, recall, and F1-scores across sentiment classes.
The linear SVM model performs well in sentiment classification, with a mean cross-validation score of around 0.71 and an accuracy of 0.71. It exhibits great precision, recall, and F1-scores across sentiment classes, particularly for positive thoughts. This indicates that sentiment classes can be effectively separated in the feature space, as well as good generalization to previously encountered data.
Despite having a mean cross-validation score of around 0.70, the decision tree model's accuracy is significantly lower at 0.63, indicating moderate performance in sentiment categorization. It struggles with negative emotions, resulting in lower precision, recall, and F1-scores in this class. Furthermore, its accuracy is lower than other models, indicating a restricted ability to identify sentiment complexity.
Random Forest: With a mean cross-validation score of around 0.73 and an accuracy of 0.74, the random forest model does well in sentiment classification. It maintains a balanced precision, recall, and F1-score across sentiment classes, showing strong and consistent results.
