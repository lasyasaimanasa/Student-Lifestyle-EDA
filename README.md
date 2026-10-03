# Student Lifestyle & Academic Performance

## Exploratory Data Analysis

### Project Overview

This project performs Exploratory Data Analysis (EDA) on student lifestyle and academic performance data.

The analysis explores how lifestyle factors such as study hours, sleep, physical activity, social hours, extracurricular activities, and stress level are associated with students' GPA.

The project focuses on understanding patterns and relationships in the dataset using descriptive analysis and visualization. No machine learning models are used.

---

## Objective

The main objective of this project is to explore student lifestyle patterns and their relationship with academic performance using Exploratory Data Analysis.

The analysis includes:

- Data understanding
- Data cleaning
- Univariate analysis
- Bivariate analysis
- Multivariate analysis
- Correlation analysis
- Outlier analysis
- Data visualization
- Key insights and conclusion

---

## Dataset

The dataset used in this project is the **Student Lifestyle Dataset** obtained from Kaggle.

According to the Kaggle dataset description, the dataset contains 2,000 student records and information related to study, extracurricular activities, sleep, social activities, physical activity, GPA, and stress level.

### Dataset Source

[Student Lifestyle Dataset - Kaggle](https://www.kaggle.com/dsv/9876359)

### Dataset Variables

| Variable | Description |
|---|---|
| Student_ID | Unique identifier for each student |
| Study_Hours_Per_Day | Daily study hours |
| Extracurricular_Hours_Per_Day | Daily extracurricular activity hours |
| Sleep_Hours_Per_Day | Daily sleep hours |
| Social_Hours_Per_Day | Daily social activity hours |
| Physical_Activity_Hours_Per_Day | Daily physical activity hours |
| GPA | Grade Point Average |
| Stress_Level | Student stress category |

---

## Research Questions

This analysis investigates the following questions:

1. How are students' daily study hours distributed?
2. How is GPA distributed among the students?
3. Is there an observable relationship between study hours and GPA?
4. Does GPA vary across different sleep durations?
5. How is physical activity associated with GPA?
6. How does GPA vary across different stress levels?
7. What relationships exist among the different lifestyle variables?

---

## Data Cleaning

The dataset was checked for common data-quality issues.

- No missing values were found.
- No duplicate rows were found.
- No negative numerical values were detected.
- The `Stress_Level` variable contains Low, Moderate, and High categories.
- Numerical variables were already stored using appropriate numerical data types.
- No major data-cleaning transformations were required.

The original observations were retained for the analysis.

---

## Exploratory Data Analysis

### Univariate Analysis

The following variables were examined individually:

- Study Hours Per Day
- GPA
- Stress Level

Visualizations were used to understand their distributions.

### Bivariate Analysis

Relationships between individual variables were explored using:

- Study Hours vs GPA
- Sleep Hours vs GPA
- Physical Activity Hours vs GPA
- Stress Level vs GPA

### Multivariate Analysis

Multiple variables were examined together using:

- Correlation heatmap
- Study Hours vs GPA grouped by Stress Level
- Average GPA across Stress Levels

### Outlier Analysis

The IQR method was used to identify potential outliers in GPA.

Four potential GPA outliers were identified:

- 4.00
- 2.25
- 2.24
- 2.25

These observations were retained because they fall within the recorded GPA range and were not identified as obvious data-entry errors.

---

## Key Findings

### 1. Study Hours and GPA

Study Hours Per Day showed the strongest positive association with GPA, with a correlation of approximately **0.73**.

### 2. Physical Activity and GPA

Physical Activity Hours Per Day showed a moderate negative association with GPA, with a correlation of approximately **-0.34**.

### 3. Sleep and GPA

Sleep Hours Per Day showed very little linear relationship with GPA.

### 4. Stress Level and GPA

GPA distributions differed across the stress-level groups.

In this dataset, the High stress group had a higher average GPA than the Moderate and Low stress groups.

This represents an observed association and does not establish that stress causes changes in GPA.

### 5. Social and Extracurricular Activities

Social Hours and Extracurricular Hours showed relatively weak relationships with GPA.

### 6. GPA Outliers

Four potential GPA outliers were identified using the IQR method and were retained for further analysis.

---

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure

```text
Student-Lifestyle-EDA/
│
├── EDA_Mini_Project.ipynb
├── student_lifestyle_dataset.csv
├── README.md
└── .gitignore
```

---

## Conclusion

The exploratory data analysis provided an overview of the relationship between student lifestyle factors and academic performance.

Among the variables examined, Study Hours Per Day showed the most noticeable positive association with GPA. Physical Activity Hours Per Day showed a moderate negative association, while Sleep Hours, Social Hours, and Extracurricular Hours showed weak or very small linear relationships with GPA.

The analysis also showed differences in GPA across stress-level groups. However, these findings represent associations observed in the dataset and should not be interpreted as causal relationships.

Overall, the project demonstrates how Exploratory Data Analysis can be used to understand patterns and relationships within student lifestyle and academic performance data.

---

## Note

This project is intended for educational and exploratory purposes. The findings describe patterns observed in the dataset and should not be interpreted as causal or predictive conclusions.
