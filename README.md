# Protct Your Tomorrow Insurance Company - Data Privacy and ML Analysis Project

### Problem Context:
Development of a comprehensive machine learning system for insurance company tasks while implementing data obfuscation techniques to protect customer privacy, addressing customer similarity analysis, payment prediction, and secure data processing.

### Objective:
Build ML models for customer analysis and payment prediction while developing data obfuscation algorithms that maintain model performance without compromising personal information privacy.

Technical Competencies Used:
Exploratory Data Analysis (EDA):
- Investigation of insurance dataset with 5,000 customer records
- Analysis of customer demographics, income, family size, and insurance benefits
- Data quality assessment and type conversions

Machine Learning - Customer Similarity (Task 1):
- k-Nearest Neighbors (k-NN): Customer similarity identification
- Distance metrics comparison (Euclidean vs Manhattan)
- Data scaling impact analysis using MaxAbsScaler
- Feature scaling effects on distance-based algorithms

Machine Learning - Classification (Task 2):
- Binary classification: Insurance payment prediction
- k-NN Classifier: Performance evaluation with F1-score
- Dummy model comparison: Random baseline with multiple probability thresholds
- Class imbalance analysis (564 vs 4,436 samples)

Machine Learning - Regression (Task 3):
- Custom Linear Regression: Matrix-based implementation using analytical solution
- Mathematical formulation: w = (X^T X)^(-1) X^T y
- RMSE evaluation for model performance assessment

Data Obfuscation & Privacy Protection (Task 4):
- Matrix transformation: X' = X × P using invertible random matrix P
- Mathematical proof: Analytical demonstration that obfuscation preserves model performance
- Data recovery: Verification of invertibility and data reconstruction
- Privacy preservation: Customer data protection without model degradation

Advanced Mathematical Analysis:
- Matrix operations and linear algebra applications
- Analytical proofs of mathematical equivalence
- Numerical precision analysis and error handling

### Main Libraries:
- pandas: Data manipulation and preprocessing
- numpy: Matrix operations and mathematical computations
- scikit-learn: Machine learning algorithms and preprocessing
  - NearestNeighbors, KNeighborsClassifier
  - MaxAbsScaler, evaluation metrics
- seaborn: Data visualization and exploratory analysis

### Final Results:
Successful implementation of privacy-preserving machine learning system:

Customer Similarity Analysis:
- Effective k-NN implementation with distance metric comparison
- Demonstrated scaling importance for distance-based algorithms
- Similar results between Euclidean and Manhattan metrics on scaled data

Payment Prediction:
- Binary classification with F1-score evaluation
- Comparison between k-NN and random baseline models
- Analysis of class imbalance effects on model performance

Linear Regression:
- Custom implementation achieving RMSE: 0.34, R²: 0.66
- Matrix-based analytical solution for optimal performance
- Consistent results across original and scaled data

Data Obfuscation Achievement:
- Mathematical proof: Analytical demonstration that X'w_P = Xw
- Computational verification: Identical RMSE and R² scores for obfuscated data
- Privacy protection: Complete data transformation while preserving model accuracy
- Invertible transformation: Successful data recovery with P^(-1)

Business Impact:
- Enables privacy-compliant machine learning operations
- Supports LGPD and data protection regulation compliance
- Maintains full model performance while protecting customer information
- Provides framework for secure data sharing and analysis
