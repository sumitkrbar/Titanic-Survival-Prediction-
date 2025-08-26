# 🚢 Titanic Survival Prediction using Machine Learning

This project applies **machine learning techniques** to predict whether a passenger survived the Titanic disaster, based on demographic and travel data. Using **Logistic Regression**, the model achieves around **80.7% accuracy on training data** and **78.2% accuracy on test data**.

---

## 📊 Project Overview
- **Goal:** Predict survival outcome of Titanic passengers using their attributes.
- **Dataset:** [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)
- **Tech Stack:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

## 🔑 Steps Implemented

### 1. Importing Dependencies
- `numpy`, `pandas` for data handling
- `matplotlib`, `seaborn` for visualization
- `scikit-learn` for model building and evaluation

### 2. Data Collection & Processing
- Loaded dataset (`train.csv`) with 891 rows and 12 columns.
- Checked for missing values.
- Preprocessed by:
  - Dropping **Cabin** column (too many missing values).
  - Filling **Age** with mean.
  - Filling **Embarked** with mode.
- Encoded categorical columns (`Sex`, `Embarked`) into numeric form.

### 3. Exploratory Data Analysis
- Count plots for survival, gender distribution, and passenger class.
- Survival distribution across **sex** and **Pclass** showed clear trends (e.g., females and higher-class passengers survived more).

### 4. Feature Engineering
- Selected features: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`
- Target variable: `Survived`

### 5. Train-Test Split
- Split dataset into:
  - **Training set:** 712 samples
  - **Test set:** 179 samples
- Test size: 20%, random state: 2

### 6. Model Training
- Applied **Logistic Regression** from scikit-learn.
- Handled convergence warnings by tuning solver/iterations if needed.

### 7. Model Evaluation
- **Training Accuracy:** ~80.7%  
- **Test Accuracy:** ~78.2%

---

## 📈 Results
- Logistic Regression performed well with ~78% test accuracy.
- Survival was strongly influenced by **sex** and **passenger class**.

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/titanic-survival-prediction.git
   cd titanic-survival-prediction
