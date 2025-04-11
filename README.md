# Cosmetics-Chemical-Analysis
Data-driven analysis of cosmetic ingredients using ML for toxicity prediction and consumer safety.
# Analyzing Chemical Ingredients in Cosmetics: A Data-Driven Approach to Safety and Compliance

## Overview
This project leverages machine learning techniques to assess the safety and compliance of chemical ingredients used in cosmetic products. Utilizing data from the California Safe Cosmetics Program (CSCP), this project aims to classify cosmetic products based on chemical characteristics and predict potential health risks associated with their ingredients.

## Problem Statement
The cosmetic industry extensively uses various chemical ingredients, many of which lack comprehensive safety information. Identifying potentially toxic ingredients manually is impractical due to data inconsistencies, scale, and complexity. This project addresses these challenges through data analytics and machine learning, improving transparency and safety standards for consumers and regulators.

## Dataset
The CSCP dataset, containing detailed information about chemicals reported in cosmetic products, serves as the project's foundation. Issues such as incomplete data, inconsistent reporting, and class imbalance are addressed using rigorous preprocessing techniques.

## Machine Learning Models
The following machine learning models were evaluated:
- **Random Forest Classifier**: Chosen for its robustness, accuracy, and interpretability via feature importance.
- **Logistic Regression**: Provided insights into baseline performance and class imbalance challenges.
- **Gradient Boosting**: Handled complex interactions efficiently and performed well in terms of recall.
- **XGBoost**: Optimized for scalability, high performance, and strong regularization, particularly effective for imbalanced data.
- **LightGBM**: Selected for its speed and efficiency on high-dimensional data.
- **AdaBoost**: Improved performance by focusing on difficult-to-classify cases.
- **CatBoost**: Excelled with categorical data, achieving the highest accuracy and balanced precision-recall.
- **Decision Tree**: Used for its interpretability and simplicity, offering clear insights into feature importance.

## Best Performing Model
- **CatBoost** achieved the highest accuracy (98.99%) with excellent balance between precision and recall, particularly effective in identifying toxic chemicals.

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

## Key Insights
- Feature importance highlighted 'CasId', 'CompanyId', and 'BrandName' as significant predictors of product toxicity.
- Handling class imbalance significantly improved model predictions, particularly for minority toxic cases.

## Installation
Clone this repository and install dependencies:
```bash
git clone https://github.com/yourusername/Cosmetics-Chemical-Analysis.git
cd Cosmetics-Chemical-Analysis
pip install -r requirements.txt
```

## Usage
Run the Jupyter notebook:
```bash
jupyter notebook cosmetics_analysis.ipynb
```

## Future Improvements
- Incorporate detailed chemical concentration data.
- Improve handling of missing data using advanced imputation techniques.
- Explore deep learning models for enhanced predictive performance.

## Contributors
- Saroja Vuluvabeeti
- Sri Sakthi Thirumagal
- Pavan Sai Rayalla
- Abhinav Reddy Padamati

## References
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html)
- [Plotly Fundamentals](https://plotly.com/python/plotly-fundamentals/)

