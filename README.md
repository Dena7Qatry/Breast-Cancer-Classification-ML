# Breast-Cancer-Classification-ML
This project applies multiple machine learning algorithms to classify tumors as **Benign (0)** or **Malignant (1)** using clinical/diagnostic measurements. The primary objective is to compare different classifiers and identify the most effective model for this dataset.

## Dataset
- **Source:** [Breast Cancer Dataset](https://github.com/abdelDebug/Breast-Cancer-Dataset/)  
- **File:** `breast_cancer_dataset.csv`  
- **Features:** Various clinical or diagnostic measurements (e.g., tumor size, texture, perimeter).  
- **Target:** Diagnosis labeled as Malignant (M) or Benign (B).  

## Models Used
The following classification algorithms were trained with default hyperparameters:
- Support Vector Machine (SVM)  
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Decision Tree  
- Random Forest  
- XGBoost  

**Note:** Scaling was avoided for tree-based models (Decision Tree, Random Forest, XGBoost).  

## Data Analysis & Key Findings
- **Data Cleaning:** No missing values. Outliers were handled using winsorization (5th and 95th percentiles).  
- **Sample Size:** The dataset was relatively small.  
- **Model Optimization:**  
  - Random Forest performance slightly decreased after tuning with GridSearchCV.  
  - XGBoost performance remained stable, indicating optimal default parameters.  
- **Model Evaluation (on test set):**  
  - Accuracy: **0.94**  
  - F1-score: **0.95**  
  - AUC-ROC: **0.94**  

**Best Models:** Random Forest and XGBoost.  

## Generalizability
Given the small training dataset, further validation on larger and balanced datasets is required to improve robustness and generalizability.  

## Future Work
- **Advanced Hyperparameter Tuning:** Explore a wider range of parameters and use optimization techniques such as RandomSearchCV.  
- **Improved Feature Selection:** Address high feature correlation using neural network approaches (e.g., CNNs).  
- **Better Outlier Handling:** Experiment with different clipping thresholds beyond the 5th and 95th percentiles.  
- **Explainability:** Tree-based models (Random Forest, XGBoost) are inherently explainable, which is important for medical applications.
   ```bash
   git clone https://github.com/your-username/Breast-Cancer-Classification-ML.git
