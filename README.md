# 🎓 Student Performance Classification (ML Project)

This project analyzes how students' background factors (like gender, parental education, and test preparation) affect their academic performance. It then uses machine learning to **classify students into Low, Medium, or High performance levels**.

---

## 📊 Dataset Overview

- **Source**: [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- **Features**:
  - Gender
  - Race/ethnicity
  - Parental level of education
  - Lunch type
  - Test preparation course
- **Target Variable**:
  - `performance_level`: Categorical label (Low, Medium, High), derived from average of math, reading, and writing scores.

---

## 🎯 Project Goals

- Perform EDA to find patterns in student background vs performance
- Convert raw scores to performance categories
- Handle class imbalance in the target
- Train and compare classification models
- Evaluate model performance with metrics like accuracy, precision, recall, and confusion matrix

---

## 🛠️ Tools & Libraries Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (Logistic Regression, Random Forest, metrics)

---

## ⚙️ Classification Models Used

| Model                      | Accuracy | Notes |
|---------------------------|----------|-------|
| Logistic Regression       | **45.5%** | Best balance of precision and recall after applying `class_weight='balanced'` |
| Random Forest (balanced)  | 39.5%     | Slightly underperformed, more confused between Medium and High |

📌 Logistic Regression performed best due to class imbalance and small dataset size.

---

## 📈 Evaluation Metrics

**Logistic Regression (Balanced Weights):**
- Accuracy: `45.5%`
- Precision/Recall (Macro Avg): ~`0.48` / `0.56`
- Confusion Matrix showed better recall for Low and Medium classes

---

## 📦 How to Run This Notebook

1. Clone the repo or download the `.ipynb` file
2. Upload it to [Kaggle](https://www.kaggle.com) or open locally with Jupyter
3. Ensure the dataset is available as `StudentsPerformance.csv`
4. Run all cells to reproduce results

---

## 📌 Project Status

- ✅ Completed: EDA, classification, evaluation
- 🔜 Optional improvements:
  - Apply SMOTE oversampling
  - Tune models with GridSearchCV
  - Deploy as API (for real-world applications)

---

## 👨‍💻 Author

- **Nimish Sinkar**
- B.E. (AI & Data Science), 3rd Year
- 💡 Focused on Data Science, Machine Learning, and Analytics
- 📂 Practicing on Kaggle, looking for internship opportunities

---

⭐ If you found this helpful, feel free to star or fork the repo!
