# 🌳✨ SVM & Decision Tree Visualizations  

## 📌 Project Overview  

This project demonstrates **binary and multiclass classification** using **Support Vector Machines (SVM)** and **Decision Trees**.  
The dataset includes **2D feature datasets** for linear, RBF, and multiclass classification scenarios.  
Decision Tree **classification** and **regression** are also included.  

---

## 📂 Files & Plots  

### 📊 Plots  

| 📎 Plot                   | 📝 Description                                                                                                               |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| `plots/linear_svm.png`    | Decision boundary of **Linear SVM** on a linearly separable dataset. Shows the separating hyperplane.                         |
| `plots/linear_rbf_svm.png`| Linear SVM decision boundary for a dataset with partially nonlinear patterns.                                                 |
| `plots/rbf_svm.png`       | **RBF SVM** decision boundary capturing circular/nonlinear patterns.                                                          |
| `plots/DT_classifier.png` | Visualized **Decision Tree** classifier for binary/multiclass dataset. Nodes show feature splits, gini, and class values.     |

---

### 📑 Datasets  

* `svm_linear.csv` – 200 rows, 2 features, binary classification (linearly separable)  
* `svm_kernel.csv` – 200 rows, 2 features, binary classification (circular/nonlinear)  
* `svm_multi.csv` – 300 rows, 2 features, 3-class classification  
* `dt_class.csv` – 200 rows, 2 features + label for Decision Tree classification  
* `dt_depth.csv` – 200 rows, 2 features to demonstrate **effect of tree depth**  
* `dt_reg.csv` – 200 rows, 1 feature → 1 target with noise for **regression tree**  

---

## 🐍 Python Code  

The code includes:  

### 🔹 SVM Classification  
- Linear and RBF kernels  
- Train-test split  
- Feature scaling using `StandardScaler`  
- Decision boundaries plotted using `plt.contourf`  
- Multiclass classification with RBF kernel  
- Accuracy and confusion matrix metrics  

### 🔹 Decision Tree Classification  
- Training and evaluation  
- Visualized tree using `plot_tree`  
- Comparison of different `max_depth` values for underfitting/overfitting  

### 🔹 Decision Tree Regression  
- Regression with `DecisionTreeRegressor`  
- RMSE comparison for `max_depth = 2, 5, None`  
- Visual analysis of predictions (optional)  

---

## ▶️ How to Run  

1. 📥 Clone/download all files including `.csv` datasets and `.png` plots.  
2. ⚙️ Install dependencies:  

```bash
pip install numpy pandas matplotlib scikit-learn