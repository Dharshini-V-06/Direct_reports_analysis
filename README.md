# 📊 Direct Reports Analysis

## 📌 Project Overview

This project analyzes the **Direct Reports dataset** to understand organizational structure, reporting hierarchies, and team dynamics. The workflow covers **basic data understanding, EDA, statistics, NumPy & linear algebra, calculus, feature engineering, and SQL-like queries in Pandas**.

Dataset link: [Direct Reports Dataset](https://drive.google.com/file/d/1dye6S7qP5uflYkPZBL73hN4L1aXqC639/view?usp=sharing)

---

## 📂 Dataset Description

The dataset contains employee and manager relationships.

### Columns:

* **employee_id** → Unique employee ID
* **position** → Job title of the employee
* **managers_id** → Employee ID of the manager (`NULL` if top-level employee)

---

## 🛠️ Project Steps

### **Part 1 – Basic Data Understanding (Pandas)**

* Load dataset into a Pandas DataFrame.
* Display first 10 rows.
* Show dataset shape, column names, and data types.
* Check for missing values & duplicates.
* Generate summary statistics with `.describe()`.

---

### **Part 2 – Exploratory Data Analysis (EDA)**

* Identify employees with `"Manager"` in their job title.
* Count number of direct reports per Manager.
* Find Manager with the **most direct reports**.
* Plot **Bar Chart**: Manager vs. Number of Direct Reports.

---

### **Part 3 – Statistics**

* Calculate **average direct reports per Manager**.
* Find **median & mode** of direct report counts.
* Probability: Randomly pick an employee → what’s the chance they report to the **CTO**?

---

### **Part 4 – Linear Algebra & NumPy**

* Represent direct reports count as a **NumPy array**.
* Create a constant weight vector to simulate **Manager Influence Score**.
* Perform vector addition & subtraction.
* Compute **dot product** between direct reports & influence score.
* Perform **matrix multiplication** for weighted sum → Manager Impact Values.

---

### **Part 5 – Calculus (SymPy)**

Model:
[
\text{Productivity Score} = \frac{\text{Direct Reports} \times \text{Efficiency Factor}}{\text{Manager Experience}}
]

* Find derivative of Productivity Score w.r.t **Direct Reports** using SymPy.
* Interpret the derivative → measures how productivity changes with team size.

---

### **Part 6 – Feature Engineering**

* Add **Direct_Reports_Count** column for each Manager.
* Create **Is_Manager** column (1 if job title contains “Manager”, else 0).
* Create **High_Team_Size** column (1 if direct reports above average, else 0).
* Rank Managers by number of direct reports.

---

### **Part 7 – SQL Simulation in Pandas**

* Find all Managers with **>3 direct reports**.
* Sort Managers by **number of reports (desc)** and **employee_id (asc)**.

---

### **Part 8 – Insights**

* Which Manager has the **largest team**?
* What is the **average team size**?
* Which Managers have **below-average team size**?
* Correlation check → Does job title type (“Data Science Manager” vs “Engineering Manager”) relate to team size?

---

## 📊 Tools & Libraries

* **Python**: pandas, numpy, matplotlib, seaborn
* **SymPy**: for symbolic calculus
* **NetworkX** (optional): for hierarchy visualization
* **Jupyter Notebook / VS Code**

---
