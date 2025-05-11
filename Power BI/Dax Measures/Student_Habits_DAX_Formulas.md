
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
