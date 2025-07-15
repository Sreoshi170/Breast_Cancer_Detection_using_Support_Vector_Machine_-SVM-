

# 🎗️ Breast Cancer Detection using Support Vector Machine (SVM)

This project uses **Support Vector Machines (SVM)** to detect breast cancer (malignant or benign) based on a variety of cell features. Both **linear** and **RBF (Gaussian)** kernels were used, along with **hyperparameter tuning**, **cross-validation**, and **decision boundary visualization**.

---

## 📊 Dataset Overview

* **Source:** Breast Cancer Wisconsin (Diagnostic) Dataset
* **Samples:** 569
* **Features:** 30 numeric features (e.g., radius, texture, perimeter, area)
* **Target:** `diagnosis` — `M = Malignant`, `B = Benign`

---

## ✅ Project Workflow

### 1. Data Preprocessing

* Dropped non-informative `id` column
* Converted `diagnosis` to binary (`M=1`, `B=0`)
* Standardized features using `StandardScaler`
* Split dataset into **80% train / 20% test**

### 2. Model Training

* Trained **SVM with Linear Kernel**
* Trained **SVM with RBF Kernel**

### 3. Model Evaluation

* **Both models achieved 100% accuracy on the test set**
* Perfect **confusion matrix** and **classification report**
* Visualized **decision boundaries** in 2D using selected features

### 4. Hyperparameter Tuning

* Performed **GridSearchCV** for RBF SVM:

  * Best parameters: `C = 10`, `gamma = 0.01`
  * Best CV Accuracy: **100%**

### 5. Cross-Validation Results

| Model      | Mean Accuracy | Std. Deviation |
| ---------- | ------------- | -------------- |
| Linear SVM | 100.00%       | ± 0.00         |
| RBF SVM    | 99.65%        | ± 0.70         |

---

## 🔧 Technologies Used

* Python
* Scikit-learn
* Pandas, NumPy
* Matplotlib, Seaborn

---

## 📈 Results

* ✅ **100% test accuracy** with both linear and RBF kernels
* ✅ High generalization confirmed through **5-fold cross-validation**
* ✅ Intuitive visualizations of **decision boundaries**
* ✅ Successfully tuned SVM parameters using GridSearch

---

## 🔗 Notebook Access

Access the full notebook here:
👉 [Open in Colab](https://colab.research.google.com/drive/1YvKiyXxfZlNI4Oj-O9jtOdWedkjM_ank)

