# 🧠 Product Sales Prediction using Advertising Data

## 👨‍💻 Author
- **Name:** Sujit Rakshe
- **Class:** SYMSc (Computer Science)
- **College:** MIT ACSC, Alandi

---

## 🏢 Vulpinix Productions LLP – Technical Assessment Round
**AI / Machine Learning Interns**

### Task
“Develop a Small Data Analysis or Prediction Model.”

---

## 📘 Project Overview
This project focuses on predicting product sales based on advertising investments across different media — TV, Radio, and Newspaper.

The goal is to understand how different advertising channels influence product sales and build a simple Machine Learning Regression Model to predict sales trends.

---

## 📊 Dataset Information
- **Dataset Name:** Advertising Dataset
- **Source:** [Kaggle – Advertising Dataset](https://www.kaggle.com/datasets/ashydv/advertising-dataset)
- **Features:**
  - `TV`: Advertising budget spent on TV (in thousands of dollars)
  - `Radio`: Advertising budget spent on Radio (in thousands of dollars)
  - `Newspaper`: Advertising budget spent on Newspaper (in thousands of dollars)
  - `Sales`: Units sold (in thousands) (target variable)

---

## 🧩 Methodology

### 1. Data Analysis (EDA)
- Calculated the correlation between advertising features and Sales:
  - **TV:** `0.90` → Strong positive correlation
  - **Radio:** `0.35` → Moderate positive correlation
  - **Newspaper:** `0.16` → Weak positive correlation
- Found that TV advertising has the highest impact on Sales.

### 2. Model Building
- Used **Linear Regression** from `scikit-learn`.
- Split the dataset into **80% Training** and **20% Testing** sets.

### 3. Model Evaluation
- **R² Score:** `0.9059` → The model explains approximately 90.6% of the variance in Sales.
- **Mean Squared Error (MSE):** `2.9078`

---

## 📈 Results

| Feature   | Coefficient |
|-----------|-------------|
| TV        | 0.0545      |
| Radio     | 0.1009      |
| Newspaper | 0.0043      |
| Intercept | 4.7141      |

### Interpretation:
- Every additional $1,000 spent on **TV ads** is associated with an increase in sales of approximately **54.5 units**.
- Every additional $1,000 spent on **Radio ads** is associated with an increase in sales of approximately **100.9 units**.
- **Newspaper ads** have a minimal impact on sales according to this model.

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn (for visualization)

---

## 💡 Conclusion

- Advertising via **TV** and **Radio** are the most effective channels for boosting sales in this dataset.
- A simple **Linear Regression** model provided strong predictive performance with a high R² score (~0.91).
- This project successfully demonstrates a basic Machine Learning workflow, from Exploratory Data Analysis (EDA) and model training to evaluation and drawing actionable insights.
