# ⚽ Football Striker Classification using Data Analytics & Machine Learning

This project analyzes a dataset of 500 football strikers using Python-based data science techniques to uncover patterns in player performance. By cleaning, visualizing, and modeling the data, it classifies strikers into **Best Strikers** and **Regular Strikers** using clustering and logistic regression.

---

## 📌 Objectives

- Identify performance attributes that define a top striker.
- Use clustering to segment players based on contribution scores.
- Build a machine learning model to predict striker type.

---

## 🧰 Tools & Technologies

| Category       | Tools/Packages                     |
|----------------|------------------------------------|
| Programming    | Python (Jupyter Notebook)          |
| Data Handling  | pandas, numpy                      |
| Visualization  | matplotlib, seaborn                |
| ML & Modeling  | scikit-learn (KMeans, LogisticRegression) |

---

## 🗃️ Dataset Overview

The dataset contains **500 football strikers**, with the following key features:

- **Performance metrics**: Goals Scored, Assists, Shots on Target, Shot Accuracy, Dribbling Success, etc.
- **Player attributes**: Nationality, Footedness, Marital Status, Consistency, Versatility, etc.
- **Behavioral data**: Hold-up Play, Big Game Performance, Off-field Conduct

---

## 🔍 Workflow Summary

### 1. 🧹 Data Cleaning
- Handled missing values using `SimpleImputer` (median for numeric, most frequent for categorical).
- Converted key columns to integer datatypes.

### 2. 📊 Exploratory Data Analysis
- Descriptive stats for key features.
- Pie and count plots for `Footedness` and `Nationality`.

### 3. 📈 Statistical Analysis
- ANOVA test to compare consistency across nationalities.
- Correlation between hold-up play and consistency.
- Linear regression to test influence of features on striker consistency.

### 4. 🧪 Feature Engineering
- Created a new feature: `Total Contribution Score`
- Encoded categorical variables (`Footedness`, `Marital Status`, `Nationality`)

### 5. 📉 Clustering (KMeans)
- Used Elbow Method to find optimal clusters (k=2)
- Segmented players into:
  - `Best Strikers` (label 1)
  - `Regular Strikers` (label 0)

### 6. 🤖 Machine Learning Model
- Logistic Regression classifier to predict striker type
- Feature scaling and train-test split
- Model evaluated using:
  - Accuracy score
  - Confusion matrix

---

## 📈 Results

- Achieved high accuracy in classification using a simple logistic regression model.
- Gained actionable insights for scout/recruitment teams on identifying high-value striker profiles.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `striker_analysis.ipynb` | Jupyter Notebook containing full analysis |
| `striker_dataset.csv` | Dataset of 500 football strikers (if available) |
| `README.md` | Project documentation (this file) |
| `requirements.txt` | (Optional) Python dependencies for reproducibility |

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/KarthigaAditya/football-striker-analysis.git
   cd football-striker-analysis
