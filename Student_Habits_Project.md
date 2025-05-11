
## 📊 DAX Measures Used

### 🔹 Key Performance Indicators (KPIs)
```dax
Average Exam Score = AVERAGE('StudentData'[Exam_Score])
Average Study Hour = AVERAGE('StudentData'[Study_Hour])
Average Sleep Hour = AVERAGE('StudentData'[Sleep_Hour])
Average Attendance = AVERAGE('StudentData'[Attendance])
```

### 🔹 Gender % Breakdown
```dax
% by Gender = 
DIVIDE(
    COUNTROWS('StudentData'),
    CALCULATE(COUNTROWS('StudentData'), ALL('StudentData'[Gender]))
)
```

### 🔹 Average Score by Groupings
```dax
Avg Score by Parental Education = AVERAGE('StudentData'[Exam_Score])
Avg Score by Sleep Hour Group = AVERAGE('StudentData'[Exam_Score])
```

### 🔹 Total Count
```dax
Total Students = COUNT('StudentData'[StudentID])
```

### 🔹 Mental Health & Diet Quality %
```dax
% by Diet Quality = 
DIVIDE(
    COUNTROWS('StudentData'),
    CALCULATE(COUNTROWS('StudentData'), ALL('StudentData'[Diet_Quality]))
)
```


---


# Student Habits vs Academic Performance Dashboard

**Dashboard by:** Kehinde Ojo  
**Tool Used:** Power BI  
**Dataset Source:** Kaggle  
**Project Type:** Educational / Behavioral Data Analysis

## 📌 Overview

This dashboard project explores the relationship between students' lifestyle habits and their academic performance. By analyzing factors such as study hours, sleep duration, attendance, exercise, diet quality, and mental health, the dashboard reveals insights into how these variables influence exam scores.

## 📊 Key Metrics & Features

- Average Exam Score, Study Hours, Sleep Hours, Attendance
- Exam Score Distribution by Gender
- Impact of Parental Education Level on Performance
- Sleep & Study Hour Influence on Scores
- Mental Health vs Diet Quality
- Student-level data table showing key behavior metrics

## 🔍 Insights

- Students with 7–8 hours of sleep perform better than those with less.
- Exam scores are relatively balanced across genders.
- Mental health tends to be higher with better diet quality.
- High attendance and lower social media hours correlate with better academic performance.

## 🛠️ Tools & Techniques

- **Power BI**: Data modeling, DAX measures, interactive visuals
- **Excel/Python**: (optional) Data cleaning and preparation
- **DAX**: Custom KPIs, aggregated metrics, and calculated measures

## 👨‍💼 My Role

- Data wrangling and transformation
- Designing and developing the Power BI dashboard
- Extracting and summarizing actionable insights

## 📎 View Dashboard

[Attach a link or screenshot here]
