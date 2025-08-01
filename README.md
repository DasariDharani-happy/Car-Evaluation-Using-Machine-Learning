# Car Evaluation Using Random Forest

## Overview
This project presents a supervised machine learning approach to classify the acceptability of cars using the Random Forest algorithm. The model is trained to assess car quality based on features that are commonly considered by buyers, such as buying cost, maintenance cost, seating capacity, luggage space, and safety level.

The goal is to automate the decision-making process and provide a reliable prediction of a car's suitability, which can benefit recommendation systems, vehicle dealers, and end-users seeking guidance in their purchasing decisions.

## Objectives
- To build a multi-class classification model using Random Forest
- To evaluate the impact of different car attributes on user acceptability
- To analyze and interpret model performance using key evaluation metrics

## Dataset Details
- **Dataset Source**: UCI Machine Learning Repository  
- **Dataset Name**: Car Evaluation Dataset  
- **Number of Instances**: 1728  
- **Number of Features**: 6 categorical input features, 1 target variable  

### Feature Descriptions:
| Feature        | Description                                  |
|----------------|----------------------------------------------|
| buying         | Buying price of the car (v-high, high, med, low) |
| maint          | Maintenance cost (v-high, high, med, low)    |
| doors          | Number of doors (2, 3, 4, 5more)             |
| persons        | Capacity in terms of persons (2, 4, more)    |
| lug_boot       | Luggage boot size (small, med, big)          |
| safety         | Safety level (low, med, high)                |
| class          | Target label (unacc, acc, good, vgood)       |

## Methodology
1. **Data Preprocessing**:
   - Categorical data encoded using `LabelEncoder`
   - Dataset split into training and testing subsets

2. **Model Building**:
   - Used `RandomForestClassifier` from `scikit-learn`
   - Trained on 80% of the data and tested on 20%

3. **Evaluation Metrics**:
   - Accuracy score
   - Confusion matrix
   - Classification report (precision, recall, f1-score)

4. **Feature Importance**:
   - Evaluated contribution of each feature using built-in feature importance attributes

## Results
The Random Forest model demonstrated strong performance on the classification task:
- Achieved high accuracy in predicting car acceptability
- Handled multi-class output effectively due to ensemble learning
- Provided insights into which features most influence car evaluations

## Libraries and Tools Used
- Python 3
- pandas, numpy for data manipulation
- scikit-learn for modeling and evaluation
- matplotlib, seaborn for visualization

## Potential Applications
- Car recommendation systems
- Consumer advisory tools
- Automobile quality assessment platforms
- Pre-processing pipeline for automotive datasets



