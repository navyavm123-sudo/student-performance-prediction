# Student Performance Prediction using Random Forest Classifier

A machine learning project that predicts whether a student will pass or fail based on study behaviour and academic factors, using a dataset of 20,000 student records.

---

## About the Project

This project builds a Random Forest classifier to predict student exam outcomes from 8 study-related features. Rather than using demographic data, the model focuses purely on study behaviour — making it more actionable and fair.

---

## Dataset

**ExamScore Dataset**
- 20,000 student records
- 13 columns including study hours, attendance, sleep quality, study method, and exam score
- Target: `Result` — derived from `exam_score` (Pass = score ≥ 40, Fail = score < 40)

---

## Project Structure

```
student-performance-prediction/
│
├── student_performance_prediction.ipynb   # Main notebook
├── ExamScore.csv                          # Dataset
├── requirements.txt
└── README.md
```

---

## What's Covered

- Exploratory Data Analysis — score distribution, study hours vs score, average score by study method and difficulty
- Correlation heatmap for numerical features
- Target variable creation with pass/fail threshold
- One-hot encoding for categorical features
- Model Training — Random Forest with 100 trees
- Model Evaluation — accuracy, classification report, confusion matrix
- Feature Importance analysis

---

## Features Used

| Feature | Type |
|---------|------|
| study_hours | Numerical |
| class_attendance | Numerical |
| internet_access | Categorical |
| sleep_hours | Numerical |
| sleep_quality | Categorical |
| study_method | Categorical |
| facility_rating | Categorical |
| exam_difficulty | Categorical |

> Excluded: `student_id` (identifier), `age`, `gender`, `course` (demographic — not study behaviour)

---

## Results

| Metric | Value |
|--------|-------|
| Algorithm | Random Forest (100 trees, entropy, max_depth=5) |
| Train/Test Split | 70% / 30% (stratified) |
| Top Features | Study hours, class attendance |

---

## How to Run

1. Clone the repository
```bash
git clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Open the notebook
```bash
jupyter notebook student_performance_prediction.ipynb
```

---

## Requirements

See `requirements.txt`. Main libraries:
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## Author

**Navya V M**  
MCA Student, CUSAT  
navyavm123@gmail.com
