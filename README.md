Social Media Burnout Detection using Machine Learning and NLP

Overview
This project is a Machine Learning and Natural Language Processing (NLP)-based system designed to detect social media burnout using behavioral, psychological, and textual data. The system analyzes user activity patterns and social media text to predict burnout levels such as Low, Moderate, and High.
The project integrates feature engineering, TF-IDF vectorization, SMOTE, and machine learning classification algorithms to improve prediction accuracy.

Features
Burnout prediction using Machine Learning
NLP-based text analysis using TF-IDF
Feature engineering for mood and stress analysis
Real-time interactive prediction system
Random Forest, SVM, and Logistic Regression models
Confusion Matrix and ROC Curve visualization
Feature Importance analysis
SMOTE for handling imbalanced datasets

Technologies Used
Python
Scikit-learn
Pandas
NumPy
Matplotlib
Seaborn
imbalanced-learn
NLP (TF-IDF)
Machine Learning Models

The following models are implemented and compared:
Random Forest
Support Vector Machine (SVM)
Logistic Regression
Random Forest achieved the highest accuracy for burnout prediction.

Dataset Features
The dataset contains:

Usage Hours
Login Frequency
Sleep Hours
Stress Level
Anxiety Level
Fatigue Level
Social Media Posts/Comments

Additional engineered features:
Mood Score
Usage Score
Sleep Score
Stress Index
Burnout Score
Feature Engineering

Custom features are generated to improve prediction performance:
Mood Score
Measures emotional condition based on stress and anxiety.
Stress Index
Combines stress, anxiety, and fatigue into a single metric.
Burnout Score
A weighted score combining behavioral and psychological indicators.
NLP Processing
The project uses TF-IDF (Term Frequency–Inverse Document Frequency) for converting textual social media posts into numerical vectors for machine learning.
Evaluation Metrics

Model performance is evaluated using:
Accuracy
Precision
Recall
F1-Score
Confusion Matrix
ROC Curve
Real-Time Prediction

The project includes an interactive prediction system where users can input:
Social media usage details
Stress and anxiety levels
Recent social media post/comment
The system predicts the burnout level and provides recommendations.

Applications
Mental health monitoring
Digital well-being analysis
Behavioral analytics
Early burnout detection systems
Future Enhancements
Deep Learning models (LSTM, BERT)
Real-time web application deployment
Integration with social media APIs
Larger real-world datasets

How to Run
Install Dependencies
pip install imbalanced-learn

Run the Project
Execute the Python script or Google Colab notebook.

Author
Monika Shree R
School of Computer Science and Engineering
Vellore Institute of Technology, Vellore, Tamil Nadu, India

test results
Random Forest Performance
----------------------------------------
Accuracy : 1.0
Precision: 1.0
Recall   : 1.0
F1 Score : 1.0

Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        29
           1       1.00      1.00      1.00        22
           2       1.00      1.00      1.00        33

    accuracy                           1.00        84
   macro avg       1.00      1.00      1.00        84
weighted avg       1.00      1.00      1.00        84


SVM Performance
----------------------------------------
Accuracy : 0.9404761904761905
Precision: 0.9483082706766918
Recall   : 0.9404761904761905
F1 Score : 0.9397643723979094

Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.83      0.91        29
           1       1.00      1.00      1.00        22
           2       0.87      1.00      0.93        33

    accuracy                           0.94        84
   macro avg       0.96      0.94      0.95        84
weighted avg       0.95      0.94      0.94        84


Logistic Regression Performance
----------------------------------------
Accuracy : 1.0
Precision: 1.0
Recall   : 1.0
F1 Score : 1.0

Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        29
           1       1.00      1.00      1.00        22
           2       1.00      1.00      1.00        33

    accuracy                           1.00        84
   macro avg       1.00      1.00      1.00        84
weighted avg       1.00      1.00      1.00        84






Predicted Burnout Level:
['Moderate']

========== SOCIAL MEDIA BURNOUT DETECTION ==========
Enter daily usage hours: 3
Enter login frequency per day: 20
Enter sleep hours: 5
Enter stress level (1-10): 7
Enter anxiety level (1-10): 6
Enter fatigue level (1-10): 5
Enter recent social media post/comment: i feel okay

========== PREDICTION RESULT ==========
Predicted Burnout Level: Moderate

Recommendation:
- Balance online and offline activities
- Monitor screen time
- Maintain healthy habits

Do you want to test another user? (yes/no): no

Exiting Burnout Detection System...
