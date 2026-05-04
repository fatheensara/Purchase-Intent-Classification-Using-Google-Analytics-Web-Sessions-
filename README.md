# Purchase-Intent-Classification-Using-Google-Analytics-Web-Sessions

### 1.0 INTRODUCTION
In the digital era, e-commerce platforms generate vast amounts of session-level data. This project focuses on analyzing over 12,000 user sessions to predict the likelihood of a purchase based on "digital footprints" left behind by shoppers. By applying predictive analytics to Google Analytics metrics, we identify behavioral signals—such as page value and exit rates—that distinguish purchasing sessions from non-purchasing ones.

**Key features of this project:**
*   **Multi-Model Classification**: Implementation and comparison of Logistic Regression, SVM, Random Forest, and XGBoost.
*   **Imbalance Handling**: Utilization of SMOTE (Synthetic Minority Oversampling Technique) to address class imbalance in shopper conversion data.
*   **Behavioral Feature Analysis**: Integration of session metrics like bounce rates, page values, and product-related durations.
*   **Advanced Evaluation**: Use of ROC-AUC curves and Confusion Matrix analysis to ensure high predictive performance.

### 2.0 OBJECTIVES
***
*   Develop a classification framework to predict e-commerce purchase intent using web session data.
*   Identify key behavioral features (e.g., session duration, traffic source) that influence a user's decision to buy.
*   Evaluate and compare machine learning models to determine the most accurate predictor for online shopper behavior.

### 3.0 DATA SOURCES
***
The research utilizes the **Online Shoppers Intention Dataset** from Kaggle, capturing detailed interactions from an e-commerce platform:
*   **Behavioral Metrics**: Administrative, Informational, and ProductRelated pages and their respective durations.
*   **Web Metrics**: Bounce rates, Exit rates, and Page values derived from Google Analytics.
*   **Contextual Data**: Operating systems, browser type, region, traffic source, and temporal markers (weekend vs. weekday, special days/months).

### 4.0 PREREQUISITES & SETUP
***
To replicate the analysis, ensure the following steps are taken:
*   **Environment**: Python 3.x with a data science distribution (e.g., Anaconda).
*   **Data Cleaning**: Perform missing-value treatment (median/mode imputation) and outlier handling via Windsorization.
*   **Feature Engineering**: Apply one-hot encoding for categorical variables like `VisitorType` and `Month`.
*   **Library Installation**: `pip install xgboost scikit-learn imbalanced-learn pandas numpy matplotlib seaborn`.

### 5.0 RUNNING THE ANALYSIS
***
The project follows a systematic Big Data workflow:
1.  **Preprocessing**: Data is normalized using min-max scaling to ensure comparable ranges for distance-based methods.
2.  **Model Training**: The dataset is split into an 80% training set and a 20% testing set.
3.  **Optimization**: XGBoost and Random Forest models are tuned to capture complex non-linear relationships in behavioral data.

### 6.0 EVALUATION
***
The framework’s performance is validated through:
*   **F1 Score & ROC AUC**: The Random Forest model achieved a leading ROC AUC of 0.9262.
*   **Recall Improvement**: SMOTE application significantly improved the model's ability to detect the minority "purchase" class.
*   **Diagnostic Analysis**: Confirmed that sessions resulting in a purchase typically have lower exit rates and higher page values.

### 7.0 REQUIREMENTS
***
*   **Machine Learning**: Scikit-learn, XGBoost, SMOTE.
*   **Data Handling**: Pandas, NumPy.
*   **Visualization**: Matplotlib, Seaborn.

### 8.0 TEAM
***
*   **Noor Afiqah binti Normadi**
*   **Galeya binti Herman Gallego**
*   **Fatheen Sara Sofiah binti Romy Norfidzy**
*   **Syasya binti Syaerill**


### ***📝 AUTHOR***
***
***Fatheen Sara Sofiah binti Romy Norfidzy***

***This project is for educational purposes.***

