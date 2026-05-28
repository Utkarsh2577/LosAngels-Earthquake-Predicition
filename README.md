# Los Angeles Earthquake Classification Using Machine Learning

## Project Overview

This project focuses on classifying earthquake events in Los Angeles using machine learning classification models. The main objective is to identify earthquake categories based on seismic features and build a predictive model that can support better understanding of earthquake patterns.

The project uses the **Los Angeles Earthquake dataset** and follows the **CRISP-DM methodology** because the goal was to clearly define the problem, understand the data, prepare it for modelling, build classification models, and evaluate their performance.

Two machine learning models were implemented:

- Random Forest Classifier
- XGBoost Classifier

The final results showed that the **Random Forest Classifier achieved 96.2% accuracy**, while the **XGBoost Classifier achieved 90.8% accuracy**. Random Forest performed better overall and showed stronger classification performance.

This project demonstrates practical skills in:

- Data cleaning
- Exploratory Data Analysis
- Feature selection
- Correlation analysis
- Feature scaling
- Classification modelling
- Model comparison
- Model evaluation using accuracy, precision, recall, and F1-score

---

## Problem Statement

Earthquakes are natural disasters that can cause serious damage to lives, infrastructure, and public safety. Understanding earthquake patterns and classifying earthquake events can support disaster management, risk analysis, and emergency planning.

The main goal of this project is to answer:

**Can earthquake events in Los Angeles be classified accurately using machine learning models based on seismic features?**

---

## Dataset Description

The dataset used in this project is the **Los Angeles Earthquake dataset**.

The dataset contains earthquake-related features such as magnitude, depth, and other seismic attributes. The target variable represents earthquake class, ranging from **1 to 6**.

The dataset initially contained missing values and irrelevant features. These were handled during the data preparation stage to improve model quality and reliability.

### Dataset Details

| Item | Details |
|---|---|
| Dataset Name | Los Angeles Earthquake Dataset |
| Problem Type | Multi-class Classification |
| Target Variable | Earthquake Class |
| Target Classes | 1 to 6 |
| Models Used | Random Forest Classifier, XGBoost Classifier |
| Methodology | CRISP-DM |

---

## Features Used

The dataset contained earthquake-related features such as:

- Magnitude
- Depth
- Other seismic attributes related to earthquake events

Some irrelevant features such as latitude, longitude, and other unnecessary columns were removed because they did not add useful value for the final classification objective.

The target variable was:

- Earthquake class

The selected features were used to classify earthquake events into different categories.

---

## Tools and Technologies Used

This project was developed using:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Random Forest Classifier
- XGBoost Classifier
- StandardScaler
- Correlation Matrix
- Jupyter Notebook

---

## Methodology

This project followed the **CRISP-DM methodology**, which includes the following stages:

---

## 1. Business Understanding

The main objective of this project was to classify earthquake events using machine learning.

Earthquake classification can help in understanding seismic patterns and can support disaster management and risk analysis. By predicting earthquake categories, this project provides a foundation for better interpretation of earthquake data.

---

## 2. Data Understanding

The Los Angeles Earthquake dataset was explored to understand the available features, target variable, missing values, and overall structure.

The dataset included earthquake-related variables such as magnitude, depth, and other seismic information. The target variable was earthquake class, ranging from **1 to 6**.

Initial analysis showed that the dataset contained missing values and irrelevant columns that needed to be handled before model training.

---

## 3. Data Preparation

Data preparation was performed to make the dataset suitable for machine learning.

This step included:

- Removing irrelevant features
- Dropping missing values
- Separating input features and target variable
- Performing correlation analysis
- Splitting the dataset into training and testing sets
- Applying feature scaling using StandardScaler

Irrelevant features such as latitude and longitude were removed because they were not useful for the final classification objective.

Missing values were handled using `dropna()` to ensure the model was trained on clean records.

---

## 4. Exploratory Data Analysis

Exploratory Data Analysis was performed to understand relationships between earthquake features and the target class.

This included:

- Checking dataset structure
- Checking missing values
- Reviewing feature relationships
- Creating a correlation matrix
- Understanding feature distributions
- Identifying variables that had stronger impact on the target variable

The correlation matrix helped guide feature selection and improved understanding of the dataset.

---

## Visualizations

Visualizations were added to make the project easier to understand and to clearly show the analysis and model performance.

---

### Correlation Matrix Heatmap

The correlation heatmap shows the relationship between earthquake features and the target class. It helped identify which features had stronger relationships with earthquake classification.

![Correlation Matrix Heatmap](images/correlation_matrix_heatmap.png)

---

### Feature Distribution

The feature distribution plot shows the spread and behaviour of selected earthquake features. This helped understand the data before model training.

![Feature Distribution](images/feature_distributions.png)

---

### Random Forest Confusion Matrix

The confusion matrix shows how well the Random Forest model classified earthquake events across different classes.

![Random Forest Confusion Matrix](images/random_forest_confusion_matrix.png)

---

### Model Accuracy Comparison

This chart compares the performance of Random Forest and XGBoost.

Random Forest achieved the highest accuracy with **96.2%**, while XGBoost achieved **90.8%**.

![Model Accuracy Comparison](images/model_accuracy_comparison.png)

---

## 5. Feature Scaling

Feature scaling was applied using **StandardScaler**.

This step was important because some machine learning models are sensitive to differences in feature scale. Scaling helped ensure that each feature contributed fairly to model training.

---

## 6. Model Building

Two classification models were trained and compared.

---

### Random Forest Classifier

Random Forest was used because it is a strong tree-based ensemble model. It can handle non-linear relationships, reduce overfitting, and work well with classification problems.

In this project, Random Forest achieved the best performance.

---

### XGBoost Classifier

XGBoost was used because it is a powerful gradient boosting algorithm designed to improve prediction accuracy by learning from previous errors.

XGBoost also performed well, but its accuracy was lower than Random Forest in this project.

---

## 7. Model Evaluation

The models were evaluated using classification metrics:

- Accuracy
- Precision
- Recall
- F1-score

The final model results were:

| Model | Accuracy |
|---|---:|
| Random Forest Classifier | 96.2% |
| XGBoost Classifier | 90.8% |

The Random Forest Classifier performed better than XGBoost and achieved the highest accuracy.

---

## Key Findings

- Random Forest achieved the best performance with **96.2% accuracy**.
- XGBoost achieved **90.8% accuracy**, which was also competitive.
- Random Forest provided better balanced results across precision, recall, and F1-score.
- Feature cleaning and scaling improved the quality of model training.
- Correlation analysis helped identify useful relationships between earthquake features and earthquake class.
- The project shows how classification models can be used for seismic event analysis.

---

## Business Value

This project shows how machine learning can support earthquake data analysis and risk-related decision-making.

The model can support:

- Earthquake event classification
- Disaster management planning
- Risk analysis
- Emergency response preparation
- Seismic pattern understanding
- Data-driven public safety insights

Although this project is academic, the approach demonstrates how machine learning can be applied to real-world risk classification problems.

---

## Results

The final comparison between the two models is shown below:

| Model | Accuracy | Performance Summary |
|---|---:|---|
| Random Forest Classifier | 96.2% | Best performing model |
| XGBoost Classifier | 90.8% | Competitive but lower than Random Forest |

Random Forest was selected as the better model because it achieved higher accuracy and stronger overall classification performance.

---

## Future Improvements

Future improvements for this project include:

- Adding more earthquake-related features
- Testing additional models such as SVM, KNN, and Neural Networks
- Applying deep learning models for advanced classification
- Performing hyperparameter tuning
- Using cross-validation for stronger model validation
- Adding feature importance analysis
- Creating a dashboard to visualize earthquake patterns
- Deploying the model as a simple prediction app

---

## Project Structure

Los-Angeles-Earthquake-Classification/  
│  
├── images/  
│   ├── correlation_matrix_heatmap.png  
│   ├── feature_distributions.png  
│   ├── random_forest_confusion_matrix.png  
│   └── model_accuracy_comparison.png  
│  
├── Los_Angeles.ipynb  
├── README.md  
└── requirements.txt  

---

## How to Run the Project

1. Clone the repository.

2. Open the project folder.

3. Install the required Python libraries:

`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `jupyter`

4. Open the notebook:

`Los_Angeles.ipynb`

5. Run all notebook cells to reproduce the analysis, visualizations, model training, and model results.

---

## Requirements

Create a `requirements.txt` file with the following libraries:

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  
xgboost  
jupyter  

---

## Conclusion

This project successfully developed machine learning classification models to classify earthquake events in Los Angeles.

By following the **CRISP-DM methodology**, the project moved through business understanding, data understanding, data preparation, modelling, and evaluation.

The **Random Forest Classifier achieved 96.2% accuracy**, outperforming the **XGBoost Classifier**, which achieved **90.8% accuracy**.

Overall, this project demonstrates how machine learning can be used to classify earthquake events and support data-driven disaster risk analysis.

---

## Author

**Utkarsh Satpute**  
MSc Data Analytics  
National College of Ireland
