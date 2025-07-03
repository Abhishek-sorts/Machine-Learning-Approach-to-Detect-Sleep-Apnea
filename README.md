# Machine-Learning-Approach-to-Detect-Sleep-Apnea
# Sleep Apnea Detection Using Machine Learning 🧠💤

This project aims to develop a machine learning-based system for the early detection of **Sleep Apnea**, using pre-recorded health and lifestyle data. It uses a **Random Forest Classifier** and compares it with other popular algorithms such as SVM, KNN, and AdaBoost.

## 🔍 Project Objective
Sleep Apnea is a serious sleep disorder that often goes undiagnosed due to the high cost and complexity of traditional diagnostic methods like Polysomnography (PSG). This project provides a cost-effective and scalable alternative using ML.

## 📁 Dataset
The dataset used is a modified version of the Sleep Health and Lifestyle dataset, containing the following features:
- Age, Gender
- Sleep Duration, Quality of Sleep
- Heart Rate, Blood Pressure (Systolic/Diastolic)
- BMI Category

**Target Variable:** `Sleep Disorder`  
Classes:
- 0: No Disorder
- 1: Sleep Apnea
- 2: Insomnia

## ⚙️ Technologies & Tools
- Python (scikit-learn, pandas, matplotlib)
- SMOTE (for class balancing)
- Jupyter / Kaggle Notebook
- Random Forest, SVM, KNN, AdaBoost

## 🧪 Model Workflow

1. **Data Preprocessing**:
   - Encoded categorical variables
   - Split blood pressure into systolic & diastolic
   - One-hot encoded BMI Category
   - Removed irrelevant columns

2. **Train-Test Split**:
   - 80/20 split with stratification

3. **SMOTE**:
   - Applied to balance the dataset

4. **Model Training**:
   - Random Forest with 200 estimators
   - Comparison with SVM, KNN, AdaBoost

5. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, F1-Score
   - Confusion Matrix Visualization

6. **Real-Time Prediction**:
   - Accepts user input and returns prediction (Apnea / Insomnia / None)

## 📊 Results

| Algorithm      | Accuracy | Precision | Recall | F1-Score |
|----------------|----------|-----------|--------|----------|
| Random Forest  | ~92%     | High      | High   | High     |
| SVM            | ~88%     | Moderate  | Moderate | Moderate |
| KNN            | ~85%     | Moderate  | Lower  | Lower    |
| AdaBoost       | ~87%     | Moderate  | Moderate | Moderate |

> Random Forest outperformed other models due to its robustness, handling of feature importance, and ability to generalize on imbalanced data.


