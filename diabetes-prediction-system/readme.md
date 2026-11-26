# 🩺 Diabetes Prediction System Using Machine Learning

A Machine Learning-based Diabetes Prediction System developed using Python and the BRFSS 2015 Diabetes Health Indicators dataset. This project explores health-related indicators and compares multiple classification algorithms to predict diabetes indicators.

## 📌 Project Overview

The main objective of this project is to build a Machine Learning classification system that predicts whether a dataset record belongs to the diabetes-indicator class (0 or 1).

The project follows a complete Machine Learning workflow, including data collection, data preprocessing, exploratory data analysis (EDA), model training, model evaluation, and prediction demonstrations using hypothetical inputs.

## 🎯 Project Objectives

- Analyze diabetes-related health indicators.
- Perform data cleaning and preprocessing.
- Explore relationships between health indicators and diabetes status.
- Train multiple Machine Learning classification models.
- Compare model performance using evaluation metrics.
- Build a prediction function for hypothetical input records.

## 📂 Dataset Information

**Dataset:** Diabetes Binary Health Indicators BRFSS 2015

| Description | Information |
|---|---|
| Total Records | 253,680 |
| Total Columns | 22 |
| Input Features | 21 |
| Target Variable | `Diabetes_binary` |
| Missing Values | 0 |
| Duplicate Records | 24,206 |

### Important Features

- HighBP
- HighChol
- CholCheck
- BMI
- Smoker
- Stroke
- HeartDiseaseorAttack
- PhysActivity
- Fruits
- Veggies
- HvyAlcoholConsump
- AnyHealthcare
- NoDocbcCost
- GenHlth
- MentHlth
- PhysHlth
- DiffWalk
- Sex
- Age
- Education
- Income

**Target Variable:**
- `0` = No Diabetes Indicator
- `1` = Diabetes Indicator

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 🤖 Machine Learning Algorithms

Three classification algorithms were implemented and evaluated:

1. Logistic Regression
2. Linear Support Vector Machine (SVM)
3. Random Forest Classifier

## 📊 Model Performance Comparison

The following results were obtained from the notebook's test-set evaluation.

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 73.15% | 31.17% | 76.70% | 44.32% | 82.42% |
| Linear SVM | 72.71% | 30.89% | 77.48% | 44.17% | 82.36% |
| Random Forest | 85.99% | 49.22% | 17.41% | 25.73% | 79.98% |

### Best Model

Logistic Regression achieved the best F1-score and ROC-AUC, providing the strongest overall balance among the three models.

Linear SVM achieved slightly higher recall, while Random Forest achieved higher precision.

**Note:** The majority-class baseline achieved 86.07% accuracy. This demonstrates why accuracy alone is not sufficient for evaluating an imbalanced classification problem.

## ⚙️ Project Workflow

The project is divided into seven phases:

**Phase 1 — Setup & First Look**
- Import libraries.
- Load the dataset.
- Inspect dataset structure and information.

**Phase 2 — Exploratory Data Analysis (EDA)**
- Analyze target distribution.
- Visualize health indicators.
- Explore relationships between features.

**Phase 3 — Train/Test Split & Preprocessing**
- Separate features and target.
- Perform stratified train/test splitting.
- Apply imputation and feature scaling using pipelines.

**Phase 4 — Model Training**
- Train Logistic Regression.
- Train Linear SVM.
- Train Random Forest.

**Phase 5 — Model Evaluation**
- Calculate accuracy, precision, recall, F1-score, ROC-AUC, and PR-AUC.
- Compare model performance.
- Analyze confusion matrices.

**Phase 6 — Prediction Demo**
- Create hypothetical input records.
- Validate feature ranges and categories.
- Generate predicted classes and estimated class probabilities.

**Phase 7 — Conclusion & Reflection**
- Summarize model performance.
- Discuss important patterns and limitations.
- Explore future improvements and ethical considerations.

## 📁 Repository Structure

```text
diabetes-prediction-system/
│
├── project-2.ipynb
│
├── diabetes_binary_health_indicators_BRFSS2015(1).csv
│
└── README.md
```

## 🚀 Installation & Setup

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/diabetes-prediction-system.git
```

**2. Navigate to the project folder**

```bash
cd diabetes-prediction-system
```

**3. Install required libraries**

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

**4. Open Jupyter Notebook**

```bash
jupyter notebook
```

**5. Open the notebook**

Open `project-2.ipynb` and run the cells sequentially.

**Important:** The original notebook uses a Kaggle dataset path. When running locally, update the `pd.read_csv()` path to match the CSV file in your project folder.

## 🔮 Future Improvements

- Improve model performance using hyperparameter tuning.
- Apply SMOTE or other class-balancing techniques.
- Explore XGBoost and Gradient Boosting.
- Implement SHAP for model explainability.
- Evaluate demographic fairness.
- Improve probability calibration.
- Validate the models on independent datasets.

## ⚠️ Limitations & Disclaimer

- The dataset contains self-reported survey information from 2015.
- Survey responses may contain reporting errors.
- The dataset may not represent all demographic populations.
- Class imbalance can affect prediction performance.
- The models have not undergone independent clinical validation.
- Predicted probabilities may not remain calibrated in different populations.

**This project is developed for educational and research purposes only. It is not a medical diagnostic tool and must not be used to determine medical treatment.**

No identifiable patient data should be collected or uploaded as part of this project.

## 👨‍💻 Author

**Sonjor Ahmed**

Aspiring Machine Learning Engineer | Data Science | Artificial Intelligence | Deep Learning

GitHub: https://github.com/sonjor46

## ⭐ Support

If you find this project useful, consider giving the repository a star ⭐.

Thank you for visiting this project!

---

*Developed with Python, Machine Learning, and Data Science.*
