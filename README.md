# 🧠 Predicting U.S. Supreme Court Decisions with Machine Learning

This project investigates how **procedural elements of Supreme Court hearings**, rather than personal attributes of justices, can be used to predict the outcomes of U.S. Supreme Court decisions. Using the **Super-SCOTUS** dataset (Fang et al., 2023b), we explore multiple machine learning models to answer research questions related to legal decision-making and potential bias in the judicial process.

---

## 📌 Project Objectives

We aim to answer the following research questions:

1. **RQ1:** Does the information available prior to or during hearings help predict Supreme Court decisions?
2. **RQ2:** Do features reflecting case difficulty contribute to decision prediction?
3. **RQ3:** Does the gender of justices affect prediction accuracy, potentially indicating bias?

### 🔬 Hypotheses

- **H1:** Pre-hearing and in-hearing information improves prediction accuracy.
- **H2:** Features related to case difficulty enhance model performance.
- **H3:** Justice gender influences Supreme Court decision outcomes.

---

## 📁 Dataset

We use the **Super-SCOTUS dataset** (Fang et al., 2023b), which contains detailed metadata on U.S. Supreme Court cases — including justice demographics, case characteristics, and decision outcomes. The dataset is divided into:

- `train.jsonl` (provided in `train.zip`)
- `dev.jsonl`
- `test.jsonl`

---

## ⚙️ Methods

The machine learning pipeline includes:

- **Feature Selection:** Filtering categorical features and engineering new ones.
- **Data Preprocessing:** Handling missing values, encoding categorical variables, and feature scaling.
- **Model Training:**
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Dummy Classifier (baseline)
- **Hyperparameter Tuning:** Identifying and optimizing model parameters.
- **Model Evaluation:** Using metrics such as Accuracy, F1 Score, and Confusion Matrix.

---

## 📊 Results

Key findings include:

- Pre- and in-hearing information is useful in predicting Supreme Court rulings.
- Case difficulty features did **not** significantly improve model performance.
- Justice gender did **not** show a statistically significant effect on decisions.

(See detailed results in the [Report.pdf](Report.pdf).)

---

## 🛠 Tools & Libraries

- **Languages:** Python
- **Libraries:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
- **Environment:** Jupyter Notebook

---

## 📄 Files

- `Project.ipynb`: Jupyter notebook with code, analysis, and visualizations.
- `Report.pdf`: Written report summarizing research questions, methodology, and findings.

---

## 🚀 How to Run

1. Clone this repository or download the files.
2. Install required Python packages (see the top of `Project.ipynb`).
3. Unzip `train.zip` into the `/data` directory.
4. Open and run `Project.ipynb` in Jupyter Notebook.

---

## 🧾 Citation

If you use the **Super-SCOTUS dataset**, please cite:

> Fang, H., et al. (2023). _Super-SCOTUS: A Dataset for Supreme Court of the United States Decision Prediction_.
