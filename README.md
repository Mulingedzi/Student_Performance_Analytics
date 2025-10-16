# Student_Performance_Analytics
Student Performance Analytics 
- Investigate how student data (attendance, grades, online activity) can be analyzed to improve learning outcomes
- Research focus: identifying dropout risks, course engagement, and personalized learning.

## Project Overview
This project investigates how student data such as attendance, study habits, and online activity can be analyzed to improve academic outcomes.  
Using a machine learning model (Random Forest Classifier), the goal is to identify performance trends and predict student success levels — enabling educators to support learners proactively.

---

##  Objectives
- Analyze factors that affect student performance.
- Identify patterns between attendance, study hours, and grades.
- Predict student performance levels (Low, Average, High).
- Provide insights for early interventions and personalized learning strategies.

---

##  Dataset Description
The dataset used is **`student_performance_updated_1000.csv`**, containing 1,000 records.  
Each record represents a student's academic and behavioral data.

| Column | Description |
|---------|-------------|
| `StudentID` | Unique student identifier |
| `Name` | Student name (removed during cleaning) |
| `Gender` | Male/Female |
| `AttendanceRate` | Percentage of attendance |
| `StudyHoursPerWeek` | Average weekly study time |
| `PreviousGrade` | Previous semester’s final grade |
| `Online_Classes_Taken` | Count of online classes completed |
| `ExtracurricularActivities` | Participation in activities (Yes/No) |
| `ParentalSupport` | Support level from home |
| `FinalGrade` | Final grade in the current term |

---

##  Data Preparation
1. **Removed irrelevant columns:** `StudentID`, `Name`  
2. **Cleaned column names:** Replaced spaces and symbols with underscores.  
3. **Handled missing values:** Dropped or filled missing data.  
4. **Label encoded categorical columns:** Gender, ParentalSupport, ExtracurricularActivities.  
5. **Standardized numeric features:** AttendanceRate, StudyHoursPerWeek, PreviousGrade, Online_Classes_Taken.

---

## Exploratory Data Analysis (EDA)
- Visualized correlations between features.
- Analyzed grade distribution.
- Explored attendance and study hours vs. final grades.
- Observed relationships between demographic and engagement factors.

**Key Observations:**
- Higher attendance correlates strongly with better grades.  
- Students with consistent study hours perform better on average.  
- Parental support and extracurricular involvement influence engagement positively.

---

##  Methodology & Model
A **Random Forest Classifier** was trained to predict student performance levels categorized as:
- **Low (0–50%)**
- **Average (51–75%)**
- **High (76–100%)**

**Training Process:**
- Split dataset: 80% training, 20% testing.
- Model fitted using scikit-learn’s RandomForestClassifier.
- Performance evaluated using accuracy, confusion matrix, and classification report.

---

##  Results & Evaluation
| Metric | Value |
|---------|--------|
| Accuracy | ~85–90% (depending on split) |
| Key Predictors | AttendanceRate, StudyHoursPerWeek, PreviousGrade |

**Feature Importance Visualization:**
Attendance and study hours were the most impactful predictors of student success.

---

##  Insights
- Attendance and consistent study time significantly improve outcomes.  
- Early identification of low-attendance students can help reduce dropout risks.  
- Combining academic and behavioral data enables personalized interventions.

---

##  Technologies Used
- **Python** (pandas, numpy, matplotlib, seaborn)
- **Scikit-learn** (RandomForestClassifier, metrics)
- **Google Colab** for experimentation and visualization
- **GitHub** for version control and documentation

---
##  Future Improvements
- Expand dataset with socio-economic and mental health factors.  
- Experiment with neural networks or gradient boosting models.  
- Deploy a dashboard for live academic risk prediction.

---

##  Author
**Project by:** **  Angel Mulingedzi Rakhumba
**Module:** Data Science Applications  
**Institution:** University of Mpumalanga   
**Year:** 2025
