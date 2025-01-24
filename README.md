## Lung Cancer Prediction Analysis

### Overview

This project aims to predict lung cancer presence using various machine learning models and statistical techniques. The dataset used is survey lung cancer.csv, which includes features such as demographics, behavioral patterns, and clinical symptoms. The analysis involves data preprocessing, exploratory data analysis (EDA), and the implementation of classification models such as Logistic Regression, Random Forest, K-Nearest Neighbors (KNN), and Linear Discriminant Analysis (LDA).

## Table of Contents

-Overview
-Project Structure
-Dataset
-Installation
-Usage
-Models and Techniques
-Results
-License

### Project Structure

├── Lung_Cancer_Analysis.Rmd   # R Markdown file for the analysis
├── survey lung cancer.csv     # Dataset file
├── README.md                  # Project documentation
├── results/                   # Directory for outputs and plots
└── models/                    # Directory for saved model objects

### Dataset

Description

The dataset contains 16 features, including:

GENDER: Gender of the individual (M/F).
AGE: Age of the individual.
SMOKING: Smoking habit (Yes/No).
YELLOW_FINGERS, ANXIETY, PEER_PRESSURE, CHRONIC.DISEASE, etc.: Behavioral and clinical features.
LUNG_CANCER: Target variable indicating lung cancer presence (Yes/No).

### Source

The dataset is provided as survey lung cancer.csv. Ensure it is in the working directory for the analysis to execute correctly.

### Installation

1. Clone the repository:
git clone https://github.com/your-username/lung-cancer-prediction.git

2. Set up the required R environment:
install.packages(c("readr", "readxl", "caret", "randomForest", "pROC", "ggplot2", "reshape2", "tidyverse"))

3. Open Lung_Cancer_Analysis.Rmd in your R IDE (e.g., RStudio).
   

### Usage 

Load and preprocess the dataset:

lc_data <- read.csv("survey lung cancer.csv")

Execute the R Markdown file to run the analysis and generate results.

View outputs such as:

Plots: Age distribution, ROC curves, confusion matrices.

Model summaries and evaluation metrics.


### Models and Techniques

Logistic Regression:

Used for binary classification.

Evaluated using cross-validation and ROC-AUC metrics.

Random Forest:

Ensemble-based classifier with OOB error analysis.

Tuned using the caret package.

K-Nearest Neighbors (KNN):

Evaluated for different values of k.

ROC curve and confusion matrix visualizations provided.

Linear Discriminant Analysis (LDA):

Used for dimensionality reduction and classification.

### Results

Evaluation Metrics: Accuracy, precision, recall, and F1 score were used to evaluate model performance.

ROC-AUC:

Logistic Regression: AUC = ...

Random Forest: AUC = ...

KNN: AUC = ...

Variable importance plots highlight key predictors of lung cancer.

License

This project is licensed under the MIT License.
