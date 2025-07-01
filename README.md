# Python-DataScience
**Project Title: Smart Health Tracker Insights**

This project explores data collected from wearable fitness devices to uncover meaningful health patterns and deliver personalized wellness recommendations. The dataset comprises 30,000 entries with features including age, gender, daily steps, heart rates, hours of sleep, calorie intake, stress levels, sleep quality, activity types, and mood. Through this data, we aim to apply regression to predict sleep and calorie metrics, classification to understand mood and stress, clustering to identify user behavior patterns, and time series analysis to observe trends over time. The project combines statistical analysis and machine learning to enable data-informed health interventions. 

**Smart Health Tracker Data Set Decription:**

Age \
Gender \
Daily Steps \
Resting Heart Rate \
Active Heart Rate \
Hours of Sleep \
Daily Calorie Intake \
Stress Level (0-10 scale) \
Sleep Quality (0-100 score) \
Daily Activity Type(categorical:sedentary, moderate, intense) \
Mood (multiclass: sad, neutral, happy)  


Based on the Analysis:
I have formualted the results and insights by comparing 3 models:
**Logistic Regression** \
**Perceptron**  \
**Deep Neueral Network** \
**Summarizing Model Evaluation Metrics across : Logistic Regression, Perceptron and Deep Neuaral Networks**

## Enhanced Model Performance Comparison

| Metric           | Logistic Regression | Perceptron (Single-Layer NN) | Deep Neural Network |
|------------------|---------------------|-------------------------------|---------------------|
| **Accuracy**     | 0.8728              | 0.8752                        | 0.8715              |
| **Precision**    | 0.8409              | 0.9437                        | 0.8776              |
| **Recall**       | 0.8950              | 0.7771                        | 0.8400              |
| **F1 Score**     | 0.8671              | 0.8524                        | 0.8584              |
| **ROC AUC**      | 0.9579              | 0.9577                        | 0.9581              |
| **Confusion Matrix** | [[2747, 471], [292, 2490]] | - | - |

### 📌 Key Insights:

- **Logistic Regression**:
  - Strong overall performance with the **highest recall (0.895)**, meaning it captures most of the actual positives.
  - Slightly lower precision indicates more false positives than the perceptron.
  - Excellent ROC AUC indicates strong separability between classes.

- **Perceptron**:
  - **Highest precision (0.9437)**, meaning its positive predictions are highly reliable.
  - However, lower recall shows it misses more actual positives compared to other models.
  - Slightly higher accuracy due to conservative positive predictions.

- **Deep Neural Network**:
  - Provides a **balanced trade-off** between precision and recall.
  - F1 Score (0.8584) suggests this model generalizes well and is robust across both false positives and false negatives.
  - Highest ROC AUC (0.9581), indicating it has the best discrimination power among the three.

