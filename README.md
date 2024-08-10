# Predictive Modeling for Insulin Dosage Using Artificial Pancreas Data

## Introduction
This project aims to enhance diabetes management by utilizing data from an artificial pancreas system to predict insulin dosage timings based on glucose readings. The primary goal is to differentiate between meal-related and non-meal-related glucose fluctuations and to apply machine learning models to optimize insulin injection times, improving patient outcomes in diabetes care.

## Dataset Description
The project utilizes two main datasets:
- **InsulinData.csv**: This dataset contains manually entered meal times and carbohydrate intake, with about 40,000 rows documenting the time and amount of carbohydrates consumed.
- **CGMData.csv**: Comprising approximately 55,000 rows, this dataset features continuous glucose monitoring data, recording glucose levels every 5 minutes to provide a detailed temporal profile of glucose variations throughout the day.

## Methods and Steps
The project follows these key steps:
- **Data Preprocessing**: Filtering relevant data from both datasets, including times and carbohydrate values, and converting timestamps into a usable format for analysis.
- **Data Segmentation**: Differentiating and categorizing glucose measurements into meal-related and non-meal-related periods to train the models accurately.
- **Feature Engineering**: Extracting crucial features from the glucose measurements such as maximum, minimum, mean levels, and time-related features to capture glucose absorption rates.
- **Model Implementation**: Using supervised learning models like Decision Trees, KNN, Random Forest, and Gradient Boosting to predict meal and no-meal periods. Unsupervised learning models such as K-Means, DBSCAN, and Hierarchical Clustering are also used to analyze patterns in glucose data.

## Model Implementation
Several machine learning models were implemented to assess their effectiveness in predicting insulin dosage timings:
- **Supervised Methods**:
  - **Decision Trees**
  - **K-Nearest Neighbors (KNN)**
  - **Random Forest**
  - **Gradient Boosting**
- **Unsupervised Methods**:
  - **K-Means**
  - **DBSCAN**
  - **Hierarchical Clustering**

Models were evaluated based on their precision, recall, f1-score, and silhouette scores to ensure nuanced performance analysis.

## Findings
The project successfully perform classification for insulin dosage based on glucose fluctuations. Models like Random Forest and Gradient Boosting showed promising results in accurately distinguishing between meal and no-meal glucose changes.

## Conclusion
The predictive models developed in this project demonstrate potential in optimizing insulin therapy for diabetes patients using an artificial pancreas. The ability to predict insulin needs based on glucose data marks a significant step forward in personalized diabetes management.

## Limitations
- **Data Dependency**: The accuracy of predictions heavily depends on the quality and granularity of the glucose and insulin data.
- **Model Generalizability**: Models need to be validated on external datasets to ensure their effectiveness across different populations.

## Future Improvements
- **Data Enrichment**: Incorporating more diverse datasets to improve model robustness.
- **Algorithm Optimization**: Further tuning the models to enhance accuracy and reduce overfitting.
