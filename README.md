# Task 7: Support Vector Machines (SVM) Classification

## 📌 Objective  
The goal of this task was to understand and implement **Support Vector Machines (SVM)** for binary classification on the **Breast Cancer dataset** from Kaggle, using both linear and non-linear kernels.

---

## 🧰 Tools & Libraries Used  
- Python 3 
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  

---

## 📁 Dataset  
**Breast Cancer Dataset**  
- Features: Various cell nucleus characteristics (e.g., radius, texture, smoothness)  
- Target: Tumor class (`Malignant` or `Benign`)

---

## ✅ Steps Performed

1. **Data Loading & Preprocessing**  
   - Loaded dataset using Pandas.  
   - Handled missing values (if any) and encoded target labels.  
   - Standardized features using `StandardScaler` to normalize scales.

2. **SVM Model Training**  
   - Trained SVM with **linear kernel**.  
   - Trained SVM with **RBF (Gaussian) kernel** to capture non-linear decision boundaries.

3. **Hyperparameter Tuning**  
   - Tuned regularization parameter `C` for both kernels.  
   - Tuned `gamma` parameter for RBF kernel.  
   - Used grid search with cross-validation to find best parameters.

4. **Evaluation & Visualization**  
   - Evaluated models using accuracy and cross-validation scores.  
   - Visualized decision boundaries on a 2D PCA projection of the data.  
   - Compared performance of linear vs. RBF kernels.

---

## 📊 Results  
- Linear SVM provided a baseline classification performance.  
- RBF kernel SVM improved accuracy by capturing non-linear patterns.  
- Optimal hyperparameters (`C` and `gamma`) significantly impacted model effectiveness.  
- Visualizations showed clear separation of classes using SVM decision boundaries.

---

## 🧠 What I Learned

### 📌 SVM Fundamentals  
- SVM tries to find the **maximum margin hyperplane** that separates classes.  
- **Support vectors** are the critical data points closest to the decision boundary.

### 📌 Kernels in SVM  
- Kernels allow SVM to model **non-linear relationships** without explicit feature mapping.  
- **Linear kernel** is suitable for linearly separable data.  
- **RBF kernel** handles complex boundaries by mapping data into higher-dimensional space.

### 📌 Hyperparameters  
- `C` controls **regularization**: trade-off between margin width and classification error.  
- `gamma` controls influence range of a single training example in RBF kernel.

### 📌 Model Evaluation  
- Cross-validation is crucial to avoid overfitting and obtain robust performance estimates.  
- Decision boundary visualization aids in understanding model behavior.

### 📌 Handling Non-linearity and Overfitting  
- Kernel trick helps with non-linear data.  
- Proper tuning of `C` and `gamma` mitigates overfitting/underfitting.

---

## ❓ Interview Questions Tackled  

1. What is a support vector?  
2. What does the `C` parameter do in SVM?  
3. What are kernels, and why are they used?  
4. Difference between linear and RBF kernel?  
5. Advantages of SVM over other classifiers?  
6. Can SVM be used for regression?  
7. How does SVM handle non-linearly separable data?  
8. How is overfitting controlled in SVM?

---

## 🏁 Conclusion  
This task strengthened my understanding of SVM theory and practical application for classification problems. I learned how to implement, tune, and evaluate SVM models, and gained hands-on experience with kernel functions and visualization techniques.
