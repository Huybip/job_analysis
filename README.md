Dưới đây là một README khá đầy đủ và phù hợp để đưa lên GitHub cho dự án **IT Job Market Analysis in Vietnam**.

---

# 📊 IT Job Market Analysis in Vietnam

## 📌 Project Overview

This project analyzes the IT job market in Vietnam using a dataset containing over **85,000 job postings**. The goal is to identify hiring trends, salary patterns, required skills, and regional demand in the technology sector.

The project follows a complete Data Analytics workflow:

```text
Data Collection
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis (EDA)
      ↓
Statistical Analysis
      ↓
Data Visualization
      ↓
Business Insights
```

---

## 🎯 Objectives

This project aims to answer the following business questions:

* Which cities have the highest demand for IT professionals?
* What are the most in-demand IT skills?
* Which job positions are recruited most frequently?
* How does salary vary across different job roles?
* How does experience affect salary?
* Which skills are associated with higher salaries?
* What skill combinations appear most frequently in job descriptions?
* Does the number of required skills correlate with salary?

---

## 📂 Project Structure

```text
IT_Job_Market_Analysis/

│
├── Data_Understanding.ipynb
├── Data_Cleaning.ipynb
├── Data_Analysis.ipynb
│
├── jobs.csv
│
├── images/
│   ├── top_cities.png
│   ├── top_skills.png
│   ├── salary_distribution.png
│   ├── salary_by_experience.png
│   └── skill_heatmap.png
│
└── README.md
```

---

# 📊 Dataset

### Dataset Information

* Total Records: **85,470**
* Total Features: **11**
* File Format: CSV

### Main Columns

| Column       | Description                 |
| ------------ | --------------------------- |
| job_title    | Job position                |
| company_name | Company name                |
| city         | Job location                |
| experience   | Required experience         |
| skills       | Required skills             |
| job_fields   | Job category                |
| salary_min   | Minimum salary              |
| salary_max   | Maximum salary              |
| avg_salary   | Average salary (calculated) |

---

# 🛠 Technologies Used

### Programming Language

* Python

### Libraries

```python
pandas
numpy
matplotlib
seaborn
```

### Environment

* Google Colab

### Visualization

* Matplotlib
* Seaborn

---

# 🧹 Data Cleaning

The following preprocessing steps were performed:

### Missing Values Handling

* Filled missing values in:

  * skills
  * city
  * job_fields

### Duplicate Removal

* Removed duplicate records.

### Salary Processing

Created a new feature:

```python
avg_salary = (salary_min + salary_max) / 2
```

### Data Standardization

* Standardized text columns.
* Removed unnecessary spaces.
* Converted text to lowercase where necessary.

### Outlier Filtering

To avoid distorted visualizations:

```python
avg_salary < 100
```

was used for most salary-related analyses.

---

# 📈 Exploratory Data Analysis

## 1. Top Hiring Cities

### Objective

Identify regions with the highest recruitment demand.

### Findings

* Ho Chi Minh City dominates IT hiring.
* Hanoi ranks second.
* Da Nang is emerging as a technology hub.

---

## 2. Most Popular Job Positions

### Objective

Identify the most frequently recruited IT roles.

### Findings

Examples:

* Backend Developer
* Frontend Developer
* Full Stack Developer
* Data Analyst
* AI Engineer

---

## 3. Most In-Demand Skills

### Objective

Determine which technical skills employers request most frequently.

### Findings

Common skills include:

* Python
* SQL
* Java
* JavaScript
* React
* Docker

---

## 4. Salary Distribution

### Objective

Understand overall salary patterns.

### Findings

* Most jobs fall within the middle salary range.
* A small number of high-paying positions create salary outliers.

---

## 5. Salary by Experience Level

### Objective

Analyze how experience affects compensation.

### Findings

* Salary generally increases with experience.
* Senior positions earn significantly more than entry-level roles.

---

## 6. Salary by City

### Objective

Compare salaries across regions.

### Findings

* Major cities offer higher salaries.
* Regional differences are clearly visible.

---

## 7. Salary by Skill

### Objective

Determine which skills are associated with higher salaries.

### Findings

Skills such as:

* AWS
* Docker
* Kubernetes
* Python

often correspond to higher average salaries.

---

## 8. Skill Frequency Analysis

### Objective

Discover the most common skills in the market.

### Findings

Top skills indicate current industry demand and learning priorities for students.

---

## 9. Skill Pair Analysis

### Objective

Identify skills that frequently appear together.

### Examples

```text
Python + SQL
React + JavaScript
Docker + Kubernetes
```

### Business Value

Provides guidance on which skills should be learned together.

---

## 10. Skill Co-occurrence Heatmap

### Objective

Visualize relationships between popular skills.

### Insights

* Strong associations exist between related technologies.
* Helpful for identifying skill clusters.

---

## 11. Number of Skills vs Salary

### Objective

Analyze whether more required skills lead to higher salaries.

### Findings

Jobs requiring more technical skills generally offer higher compensation.

---

## 12. Correlation Analysis

### Variables

* salary_min
* salary_max
* avg_salary
* skill_count

### Objective

Identify relationships between numeric features.

### Findings

Positive correlations were observed between:

* Experience and salary
* Skill count and salary

---

# 📌 Key Insights

### Recruitment Demand

* Ho Chi Minh City and Hanoi account for the majority of IT job opportunities.

### Skills

* Python, SQL, and Java remain the most requested skills.
* Cloud and DevOps skills are associated with higher salaries.

### Salary

* Experience significantly impacts salary levels.
* AI and Data-related positions generally receive higher compensation.

### Learning Recommendations

For aspiring IT professionals:

1. Learn Python
2. Learn SQL
3. Learn Git
4. Learn Power BI
5. Learn Cloud Fundamentals
6. Learn Docker

---

# 🚀 Future Improvements

Future versions of the project may include:

* Web scraping from ITviec, VietnamWorks, and TopCV.
* Interactive Power BI dashboard.
* Salary prediction model using Machine Learning.
* Job recommendation system.
* Trend analysis by posting date.

---

# 👨‍💻 Author

**Huy Tran**

Information Technology Student
Phenikaa University

### Interests

* Data Analytics
* Artificial Intelligence
* Machine Learning
* Software Development

---

# ⭐ Project Outcome

This project demonstrates:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Data Visualization
* Statistical Analysis
* Business Insight Generation

and serves as a portfolio project for **Data Analyst**, **Business Intelligence Analyst**, and **Junior Data Scientist** positions.
