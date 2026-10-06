# Diabetese-Prediction-
# 🩺 Diabetes Prediction using Machine Learning

## 📌 Project Overview

Diabetes Prediction is a **Machine Learning project** that predicts whether a person is likely to have diabetes based on different medical and health-related features.

The project uses a dataset containing information such as **Glucose level, Blood Pressure, BMI, Age, Insulin, and other medical measurements**. Machine Learning algorithms are trained on this data to identify patterns and make predictions.

This project demonstrates the complete Machine Learning workflow, from **data preprocessing and analysis to model training, prediction, and evaluation**.

---

## 🎯 Objectives

The main objectives of this project are:

- To predict the possibility of diabetes using Machine Learning.
- To analyze medical features related to diabetes.
- To preprocess and clean the dataset.
- To train classification models.
- To evaluate model performance.
- To understand how Machine Learning can be applied to healthcare data.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine Learning
- **Jupyter Notebook** – Development environment

---

## 📊 Dataset

The project uses a diabetes dataset containing medical information about patients.

### Important Features

| Feature | Description |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Blood glucose concentration |
| BloodPressure | Blood pressure measurement |
| SkinThickness | Skin fold thickness |
| Insulin | Insulin level |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Diabetes-related genetic score |
| Age | Age of the patient |
| Outcome | Diabetes prediction result |

### Target Variable

**Outcome**

- `0` → No Diabetes
- `1` → Diabetes

---

## 🔄 Machine Learning Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Selection
   ↓
Data Preprocessing
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
```

---

## 🧹 Data Preprocessing

Before training the model, the dataset is prepared using different preprocessing techniques.

### 1. Handling Missing Values

Missing or invalid values are identified and handled appropriately.

### 2. Exploratory Data Analysis

The dataset is analyzed using:

- Histograms
- Box plots
- Correlation heatmaps
- Distribution plots

### 3. Feature Scaling

Features may have different ranges. Scaling helps Machine Learning algorithms work more effectively.

For example:

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
```

### 4. Train-Test Split

The dataset is divided into training and testing data.

```python
from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
```

---

## 🤖 Machine Learning Algorithms

The project can use different classification algorithms, such as:

### 🔹 Logistic Regression

Logistic Regression is commonly used for binary classification problems. It predicts whether the patient belongs to the diabetes or non-diabetes class.

### 🔹 K-Nearest Neighbors (KNN)

KNN predicts the class of a new patient based on the classes of nearby patients in the dataset.

### 🔹 Decision Tree

Decision Tree uses a tree-like structure to make predictions based on different medical features.

### 🔹 Random Forest

Random Forest combines multiple decision trees to improve prediction performance and reduce overfitting.

---

## 📈 Model Evaluation

The trained model is evaluated using different classification metrics.

### Accuracy

Measures the percentage of correct predictions.

### Precision

Measures how many predicted diabetic cases are actually diabetic.

### Recall

Measures how many actual diabetic cases are correctly identified.

### F1-Score

Provides a balance between precision and recall.

### Confusion Matrix

A confusion matrix shows:

- True Positive
- True Negative
- False Positive
- False Negative

Example:

```python
from sklearn.metrics import accuracy_score, classification_report

print("Accuracy:", accuracy_score(y_test, y_pred))
print(classification_report(y_test, y_pred))
```

---

## 📊 Data Visualization

Visualization is used to understand relationships between different features.

Examples include:

- Glucose distribution
- BMI distribution
- Age distribution
- Diabetes outcome count
- Correlation heatmap
- Feature relationships

Example:

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.heatmap(data.corr(), annot=True)
plt.show()
```

---

## 💻 Sample Prediction

After training the model, new patient information can be given to predict the outcome.

```python
prediction = model.predict(new_data)

if prediction[0] == 1:
    print("Diabetes Predicted")
else:
    print("No Diabetes Predicted")
```

---

## 📁 Project Structure

```text
Diabetes-Prediction/
│
├── dataset/
│   └── diabetes.csv
│
├── Diabetes_Prediction.ipynb
│
├── README.md
│
└── requirements.txt
```

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Diabetes-Prediction.git
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Diabetes_Prediction.ipynb
```

---

## 📌 Results

The trained Machine Learning model can classify patients into two categories:

```text
0 → No Diabetes
1 → Diabetes
```

The performance of different models can be compared using **Accuracy, Precision, Recall, F1-Score, and Confusion Matrix**.

The best-performing model can then be selected for the final prediction system.


## 🚀 Future Improvements

This project can be improved by:

- Using larger and more diverse datasets.
- Applying advanced Machine Learning algorithms.
- Performing hyperparameter tuning.
- Using feature selection techniques.
- Creating a web application using **Streamlit**.
- Deploying the model on a cloud platform.
- Adding a user-friendly interface for predictions.
- Comparing multiple Machine Learning models.

---

## ⚠️ Disclaimer

This project is developed for **educational and Machine Learning purposes only**. The prediction generated by the model should **not be considered a medical diagnosis**. Medical decisions should always be made with the help of a qualified healthcare professional.

---

## 📚 Learning Outcomes

Through this project, I learned:

- Data preprocessing
- Exploratory Data Analysis
- Data visualization
- Classification algorithms
- Feature scaling
- Train-test splitting
- Model training
- Model prediction
- Model evaluation
- Confusion matrix
- Precision, Recall, and F1-score
- Applying Machine Learning to healthcare datasets

---

## 👨‍💻 Author

**Manali Kachale**

## ⭐ Conclusion

The **Diabetes Prediction using Machine Learning** project demonstrates how classification algorithms can be used to analyze medical data and predict the likelihood of diabetes.

The project provides practical knowledge of the complete Machine Learning pipeline, including **data preprocessing, visualization, model building, prediction, and evaluation**.

If you find this project useful, please ⭐ **Star this repository**.
