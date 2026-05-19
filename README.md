# datavisualizationasssignment
# Taxi Data Analysis using Python

## Project Overview
This project performs **data cleaning, analysis, and visualization** on the `taxis` dataset available in the Seaborn library.  
The project demonstrates how to handle missing values and create different visualizations using **Matplotlib**, **Pandas Plot**, and **Seaborn**.

---

## Dataset
The dataset used in this project is the **Taxis Dataset** from the Seaborn library.

Dataset loaded using:

```python
import seaborn as sns

df = sns.load_dataset("taxis")
```

---

# Objectives

- Load and explore the taxis dataset
- Handle missing values
- Perform data preprocessing
- Create visualizations using:
  - Matplotlib
  - Pandas Plot
  - Seaborn
- Understand relationships between taxi trip variables

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

# Project Structure

```bash
Taxi-Data-Analysis/
│
├── taxi_analysis.ipynb
├── README.md
└── requirements.txt
```

---

# Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Taxi-Data-Analysis.git
```

Move into the project folder:

```bash
cd Taxi-Data-Analysis
```

Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

---

# Import Libraries

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

---

# Data Cleaning

## Missing Value Handling

The following techniques were used:

### Numerical Columns
- Missing values replaced using **median**

### Categorical Columns
- Missing values replaced using **mode**

### Remaining Missing Values
- Rows with critical missing data were removed using:

```python
df.dropna()
```

---

# Visualizations

## Matplotlib / Pandas Plot

### 1. Line Chart
- Fare over time

### 2. Bar Chart
- Total fare by pickup borough

### 3. Pie Chart
- Trip distribution by payment method

### 4. Histogram
- Distribution of distance

### 5. Box Plot
- Tip distribution by pickup borough

---

# Seaborn Visualizations

## 1. Count Plot
- Number of trips by pickup borough

## 2. Scatter Plot
- Relationship between distance and fare

## 3. Heatmap
- Correlation between numerical variables

## 4. Pair Plot
- Pairwise relationships among:
  - Distance
  - Fare
  - Tip
  - Total

## 5. Violin Plot
- Fare distribution by payment method

---

# Key Insights

- Higher distances generally result in higher fares.
- Some boroughs generate more revenue than others.
- Credit card payments are more common than cash payments.
- Strong positive correlation exists between:
  - Fare
  - Distance
  - Total amount

---

# Sample Output

```python
df.head()
```

| pickup | dropoff | passengers | distance | fare |
|--------|---------|------------|----------|------|
| ... | ... | ... | ... | ... |

---

# Conclusion

This project demonstrates:
- Data preprocessing techniques
- Handling missing values
- Exploratory Data Analysis (EDA)
- Data visualization using Python libraries

It is a beginner-friendly project for learning:
- Pandas
- Matplotlib
- Seaborn
- Data Analytics

---

# Future Improvements

- Build machine learning models for fare prediction
- Add dashboard visualizations
- Deploy using Streamlit

---

# Author

**Mohamed Liyakath Ali**  
B.Tech Artificial Intelligence and Data Science Student  
Interested in Data Science and Analytics

---
