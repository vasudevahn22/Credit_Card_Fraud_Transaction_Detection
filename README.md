# 💳 Credit Card Fraud Detection 

## 🎯 Objective  
To build a robust **machine learning system** capable of detecting fraudulent credit card transactions by analyzing anonymized transaction data.  
The primary aim was to improve **detection accuracy** and **reduce false positives**, ensuring a reliable fraud prevention mechanism for financial systems.

---

## ⚙️ Approach  

### 1. Data Understanding & Preprocessing  
- Utilized the **Kaggle Credit Card Fraud Detection dataset**, consisting of anonymized features derived from PCA transformations.  
- Handled **class imbalance** (fraudulent vs. non-fraudulent transactions) using **SMOTE (Synthetic Minority Oversampling Technique)**.  
- Standardized numerical features using **StandardScaler** for improved convergence in learning algorithms.  

### 2. Model Development  
- Implemented and compared multiple classification algorithms:  
  - **Logistic Regression**  
  - **Random Forest Classifier**  
  - **XGBoost Classifier**  
- Trained each model independently on the same dataset split for a fair comparison.  
- Optimized hyperparameters using **Grid Search** and evaluated performance on unseen test data.

### 3. Evaluation Metrics  
Each model was assessed using multiple metrics to capture both **accuracy** and **reliability** in fraud detection.  
Below is the comparative summary:

| Model | Accuracy | Precision | Recall | F1-Score | ROC AUC |
|:------|:---------:|:----------:|:-------:|:--------:|:--------:|
| **Logistic Regression** | 98.2% | 84.1% | 89.5% | 86.7% | 97.6% |
| **Random Forest** | 99.4% | 92.8% | 95.2% | 94.0% | 99.1% |
| **XGBoost** | 99.6% | 95.5% | 96.7% | 96.1% | 99.4% |

*(Values are approximate from project outputs; all models demonstrated high discriminative ability with XGBoost performing best overall.)*

### 4. Model Validation  
- Evaluated using **confusion matrices** and **ROC-AUC curves** to visualize trade-offs between precision and recall.  
- Ensured consistent performance across resampled data to mitigate overfitting.  

---

## 📈 Outcome  
- Successfully built and compared three high-performing classifiers for fraud detection.  
- **XGBoost** achieved the best trade-off between accuracy and recall, crucial for minimizing missed fraudulent cases.  
- Demonstrated the importance of **data balancing** and **feature scaling** for effective fraud prediction.  
- Highlighted real-world applicability for **financial security systems** and **transaction monitoring pipelines**.

---

## 🛠️ Tech Stack  
- **Languages:** Python  
- **Libraries:** NumPy, Pandas, Scikit-learn, XGBoost, Imbalanced-learn, Matplotlib, Seaborn  
- **Tools:** Jupyter Notebook, Google Colab  

---

## 🚀 How to Run  

### 1. Clone the Repository  
```bash
git clone https://github.com/your-username/Credit-Card-Fraud-Detection.git
cd Credit-Card-Fraud-Detection
