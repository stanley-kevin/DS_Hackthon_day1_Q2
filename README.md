# 🏥 Hospital Department Resource Allocation Analysis

## 📌 Project Title

**Hospital – Which Department Needs More Resources?**

## 📖 Project Overview

A multi-speciality hospital wants to allocate staff and resources more effectively across its departments. Currently, resource allocation is largely based on historical assumptions rather than current demand and utilisation.

This project uses hospital department-wise data to analyze patient demand, treatment duration, staff availability, and equipment utilisation. The objective is to identify departments experiencing consistently high demand and resource utilisation and provide a data-backed resource allocation proposal.

---

## 🎯 Objectives

The main objectives of this project are:

* Clean and validate the hospital dataset.
* Perform Exploratory Data Analysis (EDA).
* Analyze patient volume across departments and months.
* Compare patient demand with available staff capacity.
* Identify departments with consistently high equipment utilisation.
* Investigate seasonal variations in patient arrivals.
* Calculate staff-to-patient ratios.
* Compare resource utilisation between departments.
* Determine whether resource utilisation differs significantly between departments.
* Build a Random Forest machine learning model.
* Evaluate the performance of the Random Forest model.
* Develop a practical resource allocation plan based on the analysis.

---

## 📊 Dataset

The dataset contains **1,200 hospital records** covering multiple departments over a 12-month period.

### Dataset Columns

| Column                       | Description                           |
| ---------------------------- | ------------------------------------- |
| `Month`                      | Month of the recorded observation     |
| `Department`                 | Hospital department                   |
| `Patient_Volume`             | Number of patients handled            |
| `Average_Treatment_Duration` | Average treatment duration in minutes |
| `Staff_Count`                | Number of staff members               |
| `Equipment_Utilisation`      | Percentage of equipment utilisation   |

### Departments Covered

* Emergency
* Cardiology
* Neurology
* Orthopedics
* General Medicine
* Pediatrics
* Gynecology
* Oncology

---

## 🔍 Key Analysis Areas

### 1. Patient Demand Analysis

Analyze the number of patients handled by each department and identify departments with consistently high patient volumes.

### 2. Capacity Analysis

Compare patient demand with available staff and treatment capacity.

A higher patient volume combined with limited staff may indicate resource pressure.

### 3. Equipment Utilisation

Analyze equipment utilisation percentages to identify departments where equipment is being used heavily.

Departments with consistently high utilisation may require:

* Additional equipment
* Equipment upgrades
* Better scheduling
* Additional staff

### 4. Seasonal Analysis

Analyze monthly patient arrivals to identify periods of increased demand.

This can help the hospital prepare additional resources during high-demand months.

### 5. Staff-to-Patient Ratio

Calculate the staff-to-patient ratio for each department.

```text
Staff-to-Patient Ratio = Staff Count / Patient Volume
```

A lower ratio indicates fewer staff members available per patient.

### 6. Department Comparison

Compare departments using:

* Patient volume
* Average treatment duration
* Staff count
* Equipment utilisation
* Staff-to-patient ratio

---

## 📈 Visualizations

The project will contain at least four important visualizations:

### Visualization 1 – Patient Volume by Department

A bar chart comparing total/average patient volume across departments.

### Visualization 2 – Monthly Patient Arrivals

A line chart showing changes in patient volume across the 12 months.

### Visualization 3 – Equipment Utilisation by Department

A bar chart or box plot comparing equipment utilisation between departments.

### Visualization 4 – Staff-to-Patient Ratio

A chart comparing staff availability relative to patient demand across departments.

---

## 📊 Statistical Analysis

Statistical analysis will be used to determine whether resource utilisation differs significantly between departments.

Possible methods include:

* Descriptive statistics
* Group-wise mean and median comparison
* Standard deviation
* ANOVA for comparing department means
* Correlation analysis

The statistical results will be interpreted together with the EDA findings.

---

# 🤖 Machine Learning

## Random Forest

The specified machine learning algorithm for this project is:

**Random Forest**

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees to make predictions.

### Prediction Target

The model can be used to predict whether a department is experiencing **high resource utilisation** based on available hospital operational data.

A derived target such as `High_Utilisation` can be created from equipment utilisation.

Example:

```text
High_Utilisation = 1
if Equipment_Utilisation >= selected threshold

High_Utilisation = 0
otherwise
```

### Features

Potential input features include:

* Patient Volume
* Average Treatment Duration
* Staff Count
* Month
* Department

Categorical variables such as Department and Month will be encoded before training.

---

## 🧪 Model Evaluation

The Random Forest model will be evaluated using appropriate classification metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

The results will be used to determine how effectively the model identifies high-utilisation situations.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data cleaning and manipulation
* **NumPy** – Numerical calculations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine learning
* **Jupyter Notebook / Google Colab** – Development environment

---

## 📂 Project Structure

```text
Hospital-Resource-Allocation/
│
├── README.md
│
├── data/
│   └── Hospital_Department_Resource_Allocation_1200.csv
│
├── notebooks/
│   └── hospital_resource_analysis.ipynb
│
├── visualizations/
│   ├── patient_volume_by_department.png
│   ├── monthly_patient_arrivals.png
│   ├── equipment_utilisation.png
│   └── staff_patient_ratio.png
│
└── requirements.txt
```

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Cleaning & Validation
   ↓
Exploratory Data Analysis
   ↓
Descriptive Statistics
   ↓
Demand & Capacity Analysis
   ↓
Seasonal Analysis
   ↓
Staff-to-Patient Ratio
   ↓
Department Utilisation Comparison
   ↓
Statistical Testing
   ↓
Feature Engineering
   ↓
Random Forest Model
   ↓
Model Evaluation
   ↓
Resource Allocation Proposal
```

---

## 💡 Expected Key Insights

The analysis is expected to identify:

1. Departments with the highest patient demand.
2. Departments experiencing consistently high equipment utilisation.
3. Months with increased patient arrivals.
4. Departments with lower staff-to-patient ratios.
5. Differences in resource utilisation between departments.
6. Relationships between patient volume, treatment duration, staff availability, and equipment utilisation.
7. Departments that may require additional resources based on combined demand and capacity indicators.

---

## 🏥 Resource Allocation Proposal

The final recommendation will be based on the results of the data analysis rather than historical assumptions.

Possible actions include:

* Increasing staff in high-demand departments.
* Adding or upgrading equipment where utilisation is consistently high.
* Adjusting staff schedules during seasonal demand peaks.
* Redistributing available resources between departments where appropriate.
* Improving appointment and patient-flow scheduling.
* Monitoring department utilisation regularly using data.

The final allocation proposal will be supported by the statistical analysis, visualizations, and Random Forest results.

---

## 📌 Expected Deliverables

The completed project will contain:

* ✅ Cleaned and validated dataset
* ✅ Exploratory Data Analysis
* ✅ Descriptive statistics
* ✅ 4 major visualizations
* ✅ 5–7 key insights
* ✅ Staff-to-patient ratio analysis
* ✅ Seasonal demand analysis
* ✅ Department utilisation comparison
* ✅ Statistical significance analysis
* ✅ Trained Random Forest model
* ✅ Model evaluation results
* ✅ Practical resource allocation proposal

---

## 👥 Conclusion

This project provides a data-driven approach to hospital resource planning. By analyzing patient demand, staff availability, treatment duration, and equipment utilisation, the hospital can identify areas where resources may be under pressure.

The combination of statistical analysis, visualizations, and Random Forest prediction provides a structured approach for supporting future resource allocation decisions.
#   D S _ H a c k t h o n _ d a y 1 _ Q 2  
 