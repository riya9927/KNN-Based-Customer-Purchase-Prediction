# KNN-Based-Customer-Purchase-Prediction

This project demonstrates the use of the **K-Nearest Neighbors (KNN)** algorithm to predict customer purchase behavior based on age and estimated salary using a dataset from social network ads.

---

## Project Objective

Build a predictive model that determines whether a customer will make a purchase or not, based on:
- Age
- Estimated Salary

---

## Dataset

- **Source**: `Social_Network_Ads.csv`
- **Attributes**:
  - `User ID`: Unique identifier
  - `Gender`: Male/Female
  - `Age`: Age of the customer
  - `EstimatedSalary`: Annual salary
  - `Purchased`: Target variable (0 = No, 1 = Yes)

---

## Technologies Used

- Python
- Pandas, NumPy
- Seaborn & Matplotlib
- Scikit-learn

---

## Algorithm: KNN

**Steps followed:**
1. Select optimal value for `k` (k=5 used).
2. Compute Euclidean distance for neighbors.
3. Identify `k` nearest neighbors.
4. Assign class based on majority voting.

---

## Model Performance

- **Train-Test Split**: 80:20
- **Scaling**: Performed with `StandardScaler`
- **Model**: `KNeighborsClassifier` with `metric='minkowski'`, `p=2`

### Results:

- **Accuracy**: 93.75%
