# 📊 Analysis of Mental Health's Influence on Academic Performance  

## 📺 Project Overview  
This project examines the **impact of mental health factors**—such as stress, anxiety, and depression—on **students' academic performance (CGPA)**. It also explores **demographic influences** such as **age, gender, field of study, and academic year** on mental health.  

By leveraging **data science techniques**, statistical analysis, and **machine learning**, this study aims to provide **data-driven insights** that can help support student well-being and academic success.  

---

## 📂 Data Sources  
This analysis is based on **two publicly available datasets** containing survey responses from university students in **Bangladesh** and **Malaysia**:  

1. **University Students Mental Health (Bangladesh)**  
   - **Source:** [Kaggle](https://www.kaggle.com/datasets/mohsenzergani/bangladeshi-university-students-mental-health)  
   - **License:** MIT  
   - **File:** `Raw Data.csv`  

2. **Student Mental Health (Malaysia)**  
   - **Source:** [Kaggle](https://www.kaggle.com/datasets/shariful07/student-mental-health)  
   - **License:** Public Domain (CC0)  
   - **File:** `Student Mental health.csv`  

---

## 🚀 Key Analysis & Methods  
- **Data Cleaning & Preprocessing**: Used **Pandas** to ensure accuracy and consistency in analysis.
- **Exploratory Data Analysis (EDA)**: Identified patterns in mental health and academic performance through **descriptive statistics and visualizations**.
- **Statistical Analysis**: Assessed **correlations between mental health challenges and CGPA** to pinpoint key academic stressors.
- **Demographic Insights**: Investigated the influence of **age, gender, and academic pressures** on mental health trends using **Ordinary Least Squares (OLS) regression**.
- **Data Visualization**: Created **comprehensive visual reports** to effectively communicate findings.

---

## 🛠️ Technologies & Libraries Used
- **Python**
- **Pandas, NumPy** → Data manipulation
- **Matplotlib, Seaborn** → Data visualization
- **Statsmodels** → Statistical analysis and modeling

---
## 📂 Project Structure  
📂 Data-Science-Mental-Health-CGPA-Analysis

│── 📂 data/ # Contains dataset files

│── Analysis_on_mental_health.ipynb

## 📊 Key Insights & Findings  

### **1. Impact of Demographic Factors on Mental Health**
- **Gender Differences:** Female students report significantly **higher levels of stress, anxiety, and depression** than male students. However, the dataset contains more female respondents, which may influence the observed trend.
- **Age Trends:** Younger students (18-20 years old) experience **higher stress levels**, particularly in their **first and second years** of university.
- **Year of Study:** Stress peaks in **middle academic years (2nd & 3rd year)** and slightly decreases in the final year.
- **Field of Study Influence:** **Civil Engineering students** report the **highest mental health challenges**. However, **non-engineering fields** also show significant levels of stress, particularly **Business and Entrepreneurship students**.

### **2. Mental Health & Academic Performance (CGPA)**
- **Weak correlation between CGPA and mental health factors** suggests that academic performance is influenced by additional factors not captured in this dataset.
- **Statistically significant predictors of CGPA** include:
  - **Negative Impact:** Nervousness, anger due to performance, self-doubt.
  - **Positive Impact:** Trouble relaxing, inadequate coping, fatigue.
- **Students with moderate stress may still perform well academically**, whereas severe stress correlates with lower performance.

### **3. Mental Health Trends Across Two Datasets**
- **Bangladesh Dataset:** Indicates that middle academic years (2nd & 3rd) experience the most stress, while Engineering students report the highest mental health issues.
- **Malaysia Dataset:** Suggests that **first-year students** experience the most mental distress, possibly due to university transition challenges.
- **Female students consistently report higher levels of anxiety and depression** in both datasets.

### **4. Departmental Influence on Mental Health**
- **Engineering and IT students report the highest stress levels**, but sample size imbalance prevents a strong conclusion.
- **More data is needed to determine if Engineering is inherently more stressful than other fields**.

### **5. Key Takeaways & Future Considerations**
- **Universities should focus on supporting students in their early academic years** when stress and mental health challenges peak.
- **Engineering and Business students require targeted mental health interventions** due to consistently high stress levels.
- **Further research needed** to determine additional factors affecting CGPA beyond mental health.
- **Data limitations** (skewed distributions, underrepresented groups) should be considered before generalizing findings.

---
## ▶️ How to Run the Project
### **1. Clone the Repository**
```bash
git clone https://github.com/AsenSirakov/Data-Science-Projects.git
cd Data-Science-Mental-Health-CGPA-Analysis
```

### **2. Open the Jupyter Notebook**
Launch the analysis notebook using:
```bash
jupyter notebook Analysis_on_mental_health.ipynb
```

### **3. Execute the Cells**
- Follow the **step-by-step code execution**
- **Run all cells** to see visualizations and results
