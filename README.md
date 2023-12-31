# KNN-Based Classification of Spinal Conditions in the Vertebral Column Data Set

## Overview
This project is centered around the analysis and classification of the Vertebral Column Data Set, originally compiled by Dr. Henrique da Mota. The primary focus is on binary classification of spinal conditions into Normal (NO=0) and Abnormal (AB=1), utilizing biomechanical features from the pelvis and lumbar spine. The project encompasses data pre-processing, exploratory data analysis, and classification employing the K-Nearest Neighbors (KNN) algorithm.

## Data Set Description
The data set includes patient-specific biomechanical attributes such as pelvic incidence, pelvic tilt, lumbar lordosis angle, sacral slope, pelvic radius, and grade of spondylolisthesis. Classifications include Disk Hernia (DH), Spondylolisthesis (SL), Normal (NO), and Abnormal (AB), with this project focusing on the NO and AB categories.

## Getting Started

### Data Acquisition
Download the Vertebral Column Data Set from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Vertebral+Column).

### Pre-Processing and Exploratory Data Analysis
- Generate scatterplots and boxplots for independent variables, categorized by class labels.
- Divide the dataset into training and testing sets as per specified guidelines.

### Classification with KNN
- Implement KNN classification utilizing the Euclidean metric.
- Conduct model evaluation, including the determination of the optimal k value.
- Construct learning curves to assess the influence of training set size on the model's effectiveness.

### Variants of KNN
Explore alternative distance metrics like Minkowski, Manhattan, Chebyshev, and Mahalanobis, analyzing their effect on classification accuracy.

### <strong> Analysis of Test Error Rate </strong>
#### Majority Polling Decision:
|     | Metrics                  | K*   | Test Error Rate  |
|-----|--------------------------|------|------------------|
| 0   | Manhattan                | 1    | 0.11             |
| 1   | Minkowski(log10(p)=0.7)  | 1    | 0.11             |
| 2   | Chebyshev                | 16   | 0.08             | 
| 3   | Mahalanobis              | 6    | 0.08             | 

#### Weighted Decision:
|     | Metrics    | K*   | Test Error Rate  |
|-----|------------|------|------------------|
| 0   | Euclidea   | 6    | 0.10             |
| 1   | Manhattan  | 26   | 0.10             |
| 2   | Chebyshev  | 16   | 0.11             | 


## Requirements
- Python 3.x
- Libraries: numpy, pandas, matplotlib, scikit-learn

## Installation
Install the necessary libraries using the following command:
```bash
pip install numpy pandas matplotlib scikit-learn
```

## Usage
Run the Jupyter notebook KNN-Based_Classification_Cici_Chang.ipynb to perform the analysis. The notebook contains detailed instructions and code for each step of the project.
