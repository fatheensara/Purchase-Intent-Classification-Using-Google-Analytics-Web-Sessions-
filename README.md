# Purchase-Intent-Classification-Using-Google-Analytics-Web-Sessions

### 1.0 INTRODUCTION
This project focuses on predicting e-commerce purchase intent by analyzing session-level data from the Online Shopper Intention Dataset. In the digital era, understanding consumer behavior through "digital footprints" is essential for retailers to personalize experiences and increase conversion rates. The system analyzes behavioral metrics such as bounce rates, page values, and session durations to classify whether a user will complete a transaction.

**Key features of this project:**
*   **Big Data Classification**: Statistical analysis of over 12,000 user sessions with 18 distinct behavioral and temporal features.
*   **Predictive Modeling**: Implementation of multiple machine learning algorithms including Logistic Regression, SVM, Random Forest, and XGBoost.
*   **Class Imbalance Handling**: Application of SMOTE (Synthetic Minority Oversampling Technique) to improve model recall for the minority purchase class.
*   **Interactive Analysis**: Data-driven insights into how visitor types (New vs. Returning) and traffic sources impact revenue.

### 2.0 OBJECTIVES
***
*   Develop a classification framework to reliably predict purchase intent using Google Analytics web session data.
*   Identify key features—such as exit rates and page values—that significantly influence a user's decision to purchase.
*   Compare the performance of various machine learning models to determine the most effective approach for e-commerce analytics.
*   Provide actionable insights for SMEs to improve customer segmentation and targeted advertising.

### 3.0 DATA SOURCES
***
The project utilizes the **Online Shoppers Intention Dataset** from Kaggle, which includes:
*   **Behavioral Features**: Administrative, Informational, and Product-Related page visits and durations.
*   **Web Metrics**: Bounce rates, Exit rates, and Page values.
*   **Temporal/Contextual Data**: Month of visit, Operating Systems, Browser type, Region, Traffic Type, and Weekend status.
*   **Target Variable**: Revenue (True/False).

### 4.0 PREREQUISITES
***
Before running the analysis, ensure the following steps are completed:
*   **Environment**: Install a Python 3.x environment (Anaconda or Google Colab recommended).
*   **Library Installation**: Install the necessary data science libraries:
    `pip install pandas scikit-learn xgboost imbalanced-learn matplotlib seaborn`
*   **Dataset Placement**: Ensure the file `online_shoppers_intention.csv` is in the same directory as the notebooks.
*   **Data Cleaning**: The scripts automatically handle missing value treatment (median/mode imputation) and outlier handling.

### 5.0 RUNNING THE ANALYSIS
***
The analysis is contained within the following Jupyter Notebooks:
*   **Main Model**: Run `group_project_bda_classification_model.ipynb` to execute the full machine learning pipeline, including feature encoding and model comparison.
*   **Code Implementation**: Refer to `code.ipynb` for the modular implementation of the preprocessing and training logic.

**The analysis workflow follows:**
1.  **Preprocessing**: Categorical features like `VisitorType` and `Month` are converted via Label Encoding.
2.  **Scaling**: Numerical features are normalized using `StandardScaler`.
3.  **Training**: The data is split into an 80/20 train-test ratio.
4.  **Execution**: Models are trained through a `Pipeline` to ensure data integrity.

### 6.0 EVALUATION
***
The models are evaluated using a comprehensive suite of metrics:
*   **ROC-AUC Curve**: Used to measure the model's ability to discriminate between buyers and non-buyers.
*   **F1-Score**: To assess the balance between precision and recall, especially after applying SMOTE.
*   **Performance Comparison**: In this study, the **Random Forest** model outperformed others with an **F1 score of 0.65** and an **ROC AUC of 0.9262**.
*   **Feature Importance**: Analysis confirmed that `PageValues` and `ExitRates` are the strongest predictors of purchase intent.

### 7.0 REQUIREMENTS
***
*   **Data Analysis**: Pandas, NumPy.
*   **Machine Learning**: Scikit-Learn, XGBoost.
*   **Handling Imbalance**: Imbalanced-learn (SMOTE).
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

