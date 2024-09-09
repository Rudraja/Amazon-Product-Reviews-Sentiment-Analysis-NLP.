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
### Results (Without Cross Validation)

- **Logistic Regression**:
  - Accuracy: ~70%.
  - Balanced performance across all sentiment classes.
  - Struggles with classifying negative sentiments.
  - Consistent precision, recall, and F1-score across positive and neutral sentiments.

- **Linear SVM**:
  - Accuracy: ~71%.
  - Performs better than logistic regression, especially in classifying both positive and negative sentiments.
  - Excels at classifying positive emotions.
  - Superior ability to separate sentiment classes in the feature space.

- **Decision Tree**:
  - Accuracy: ~68%.
  - Decent precision and recall for neutral sentiments.
  - Struggles with negative sentiments, leading to overall poor performance.
  - Likely overfitting, seen through fluctuating recall and precision across sentiment classes.

- **Random Forest**:
  - Accuracy: ~69%.
  - Balanced precision, recall, and F1-score across all sentiment classes.
  - Struggles with categorizing negative sentiments, reducing precision for this class.
  - Performs better than a single decision tree due to ensemble technique, minimizing overfitting issues.
    
With Cross Validation:
### Results (With Cross Validation)

- **Logistic Regression**:
  - Accuracy: 0.70
  - Mean Cross-Validation Score: 0.70
  - Balanced precision, recall, and F1-scores across all sentiment classes.
  - Consistent performance in sentiment classification.

- **Linear SVM**:
  - Accuracy: 0.71
  - Mean Cross-Validation Score: 0.71
  - Excellent precision, recall, and F1-scores, particularly for positive sentiments.
  - Effective separation of sentiment classes in the feature space.
  - Good generalization to new data.

- **Decision Tree**:
  - Accuracy: 0.63
  - Mean Cross-Validation Score: 0.70
  - Moderate performance in sentiment categorization.
  - Struggles with negative sentiments, leading to lower precision, recall, and F1-scores for this class.
  - Lower accuracy compared to other models, indicating limited ability to handle sentiment complexity.

- **Random Forest**:
  - Accuracy: 0.74
  - Mean Cross-Validation Score: 0.73
  - Strong and consistent results with balanced precision, recall, and F1-scores across sentiment classes.
  - Best overall performance among the models.
