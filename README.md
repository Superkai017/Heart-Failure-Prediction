# Heart-Failure-Prediction
# 🫀 Heart Failure Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange?style=flat-square&logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)

> A machine learning project to predict the likelihood of heart failure in patients based on clinical features — enabling early intervention and better healthcare outcomes.

---

## 📌 Overview

Heart failure is a leading cause of mortality worldwide. This project leverages supervised machine learning techniques to predict heart failure events based on patient health records, helping clinicians make faster, data-driven decisions.

The model is trained on clinical features such as age, ejection fraction, serum creatinine, and more to classify whether a patient is at risk.

---

## 📊 Dataset

- **Source**: [Heart Failure Clinical Records Dataset — UCI / Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
- **Samples**: 299 patients
- **Target Variable**: `DEATH_EVENT` (1 = death occurred, 0 = survived)

### Features

| Feature | Description |
|---|---|
| `age` | Age of the patient |
| `anaemia` | Whether the patient has anaemia |
| `creatinine_phosphokinase` | Level of CPK enzyme in the blood |
| `diabetes` | Whether the patient has diabetes |
| `ejection_fraction` | Percentage of blood leaving the heart per contraction |
| `high_blood_pressure` | Whether the patient has hypertension |
| `platelets` | Platelet count in the blood |
| `serum_creatinine` | Level of serum creatinine in the blood |
| `serum_sodium` | Level of serum sodium in the blood |
| `sex` | Patient's sex |
| `smoking` | Whether the patient smokes |
| `time` | Follow-up period (days) |

---

## 🧠 Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- XGBoost / Gradient Boosting *(if applicable)*

---

## 🏆 Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---|---|---|---|
| Logistic Regression |  | — | — | — |
| Random Forest | | — | — | — |
| SVM | | — | — | — |

> 📝 *Update the table above with your actual results after running the experiments.*

---

## 🗂️ Project Structure

```
Heart-Failure-Prediction/
│
├── data/
│   └── heart_failure_clinical_records.csv
│
├── notebooks/
│   └── EDA_and_Modeling.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── evaluate.py
│
├── models/
│   └── best_model.pkl
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/Heart-Failure-Prediction.git
cd Heart-Failure-Prediction

# Install dependencies
pip install -r requirements.txt
```

### Run the Project

```bash
# Run training
python src/train.py

# Evaluate the model
python src/evaluate.py
```

Or open the Jupyter Notebook for an interactive walkthrough:

```bash
jupyter notebook notebooks/EDA_and_Modeling.ipynb
```

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
xgboost
```

---

## 📈 Exploratory Data Analysis

Key insights from EDA:

- **Age** and **serum creatinine** are among the strongest predictors.
- **Ejection fraction** shows a clear inverse relationship with mortality.
- The dataset is slightly imbalanced (~67% survived, ~33% death events).

---

## 🛠️ Future Improvements

- [ ] Handle class imbalance using SMOTE or class weighting
- [ ] Hyperparameter tuning with GridSearchCV / Optuna
- [ ] Deploy as a web app using Streamlit or Flask
- [ ] Add SHAP values for model explainability
- [ ] Experiment with deep learning approaches

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- Dataset from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records)
- Inspired by the paper: *"Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone"* — Chicco & Jurman (2020)

---

<p align="center">Made with ❤️ for better healthcare outcomes</p>
