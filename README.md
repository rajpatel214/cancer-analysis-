# Cancer-Analysis-Project

**1. Data Exploration & Preprocessing**
Imported the dataset and checked for missing values (none found).
Performed Exploratory Data Analysis (EDA) to understand tumor characteristics.
Scaled the data using RobustScaler for better model performance.

**2. Clustering Analysis**
Applied K-Means Clustering (n=2) to group tumors based on size and texture.
Used Agglomerative Clustering to compare performance.
**Evaluated clusters using the Silhouette Score:**
**K-Means**: 0.53
**Agglomerative:** 0.49

**3. Machine Learning Models for Cancer Prediction**

Split data into training and testing sets.
Tested multiple models:
**Logistic Regression → Best performance** (98% accuracy)
**Random Forest Classifier** → 95% accuracy
**Support Vector Machine (SVM)** → 97% accuracy
**Decision Tree & KNN** → Performed lower than other models.

**4. Model Improvement with Hyperparameter Tuning**
Used RandomizedSearchCV to optimize Random Forest parameters.
Improved performance of Random Forest to 96%, but Logistic Regression remained the best model.

**5. Final Outcome & Key Insights**
Logistic Regression is the best model (98% accuracy) for predicting cancer diagnosis.
Tumor size analysis showed that most patients had an average tumor size between 12-15 units.
Clustering helped identify different tumor characteristics, supporting better diagnosis.
Feature scaling and model tuning improved overall accuracy and reliability.
