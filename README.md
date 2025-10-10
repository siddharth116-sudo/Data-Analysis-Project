# 📊 Graduate Employability Analysis & Placement Prediction

> A data-driven exploration of student performance and placement outcomes — identifying key academic and non-academic factors affecting employability, predicting placement success, and providing actionable insights for institutions and students.

---

## 👥 Team Members

* **Siddharth Magdum** 
* **Tushar Satpute** 
* **Rahul Nawale** 

---

## 🎯 Problem Statement

Despite the increasing number of graduates entering the job market, many struggle to secure suitable employment. Employers often cite mismatches between academic performance, technical skills, and employability attributes as barriers to recruitment. 

This project aims to:

* Identify **academic and non-academic factors** that most influence employability
* Predict **placement outcomes** using student performance indicators
* Explore correlations between categorical factors (e.g., gender, stream, internship experience) and placement success
* Provide **actionable insights** for universities and policymakers to improve curriculum design and career readiness programs
* Build a **data-driven framework** to enhance graduate employability and placement strategies

---

## 🗂️ Data Sources

We analyzed the **Graduate Employability Dataset (Student Performance vs Placement Dataset)**, which includes:

* **Academic Performance:** Previous semester grades, CGPA, subject scores
* **Employability Indicators:** Internships, projects completed, communication skills, extra-curricular scores
* **Placement Outcome:** Placed or not placed (target variable)
* **Demographics & Streams:** Gender, degree, specialization, location

> The dataset was cleaned, preprocessed, and prepared for modeling.

---

## ⚙️ Methodology Overview

### **Phase 1 – Data Cleaning & Pre-processing (Completed)**

* Handled missing values, duplicates, and outliers
* Standardized categorical columns (stream, degree, gender)
* Normalized numeric features (CGPA, skill scores)
* Exported processed dataset for modeling (`processed_data.csv`)

### **Phase 2 – Exploratory Data Analysis (Completed)**

* Univariate, bivariate, and multivariate analysis
* Identified key trends and correlations between features and placement outcomes
* Visualized distributions, skill gaps, and placement patterns
* Derived insights such as:

  * Higher CGPA and strong communication skills increase placement probability
  * Internship experience strongly correlates with employability
  * Certain streams and degrees show better placement rates

### **Phase 3 – Modeling & Evaluation (Completed)**

* **Predictive Modeling:** Logistic Regression, Random Forest, XGBoost
* **Feature Importance Analysis:** Identify top predictors of placement success
* **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC
* **Outputs:**

  * `models/placement_predictor.pkl`
  * `outputs/model_metrics.csv`, `outputs/feature_importance.png`

### **Phase 4 – Reporting & Visualization (Completed)**

* Created an interactive dashboard summarizing insights
* Generated plots for key findings, correlations, and placement trends
* Delivered final report (`final_report.pdf`) and presentation (`presentation.pptx`)
* Insights enable actionable strategies for students and institutions

---

## 📁 Repository Structure

```text
Data-Analysis-Project/
├── Data/
│   ├── Processed Data/
│   └── Raw Data/
│
├── Notebook/
│   ├── EDA.ipynb
│   ├── dataloading_inspection.ipynb
│   ├── featureanalysis.ipynb
│   ├── hyperparametertuning.ipynb
│   ├── installation.ipynb
│   ├── model_evaluation.ipynb
│   └── preprocessing_splitting.ipynb
│
├── Outputs/
│   ├── Confusion Matrix.png
│   ├── Histogram.png
│   ├── Numeric feature corelation.png
│   ├── ROC Curve.png
│   └── Random Forest Features.png
│
├── README.md
└── requirement.txt
---

## 🧹 Key Deliverables (Final)

| Phase  | Deliverable                                       | Status      |
| ------ | ------------------------------------------------ | ----------- |
| Phase 1 | Data cleaning & preprocessing                     | ✅ Completed |
| Phase 2 | Exploratory analysis & insights                  | ✅ Completed |
| Phase 3 | Modeling & placement prediction                  | ✅ Completed |
| Phase 4 | Dashboard, report & presentation                 | ✅ Completed |

---

## 📊 Final Outputs

* **Processed Data:** `processed_data.csv` (~36K rows)
* **Models:** `placement_predictor.pkl`
* **Reports:** `final_report.pdf`, `presentation.pptx`
* **Visuals:** `feature_importance.png`, `placement_trends_chart.png`
* **Tables:** `model_metrics.csv`, `correlation_matrix.csv`

---

## 🚀 How to Run

```bash
git clone https://github.com/siddharth116-sudo/Data-Analysis-Project.git
cd Data-Analysis-Project
pip install -r requirements.txt
