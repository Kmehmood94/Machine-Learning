Breast Cancer Detection using Wisconsin Dataset

Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Model Evaluation](#model-evaluation)
- [Deployment](#deployment)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

Introduction

This repository contains an end-to-end machine learning project aimed at detecting breast cancer using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset. The primary objective is to build a predictive model that can accurately classify tumors as benign or malignant based on various features extracted from digitized images of fine needle aspirates (FNA) of breast masses.

Dataset

The dataset used in this project is the **Wisconsin Diagnostic Breast Cancer (WDBC) dataset**, which is publicly available on [Kaggle](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data). It contains 569 samples of tumors, with 30 features representing different characteristics of cell nuclei, such as radius, texture, and smoothness. The target variable is binary, indicating whether the tumor is benign (0) or malignant (1).

- **Number of Instances:** 569
- **Number of Features:** 30
- **Target:** Binary (0 - Benign, 1 - Malignant)

## Project Structure

```
├── data
│   ├── data.csv          # The dataset used for this project
├── notebooks
│   ├── ML_Project_Breast_Cancer_Detection.ipynb  # Data preprocessing steps,  FastAPI app for deployment                              
├── README.md                      # Project overview
├── LICENSE                        # License information
└── .gitignore                     # Files and directories to ignore in Git

## Data Preprocessing

The preprocessing steps include handling missing values, normalizing the features, and splitting the data into training and testing sets. The preprocessing code can be found in the `01_data_preprocessing.ipynb` notebook.

## Exploratory Data Analysis (EDA)

EDA was performed to understand the distribution of features and their relationships with the target variable. Key insights and visualizations can be found in the `ML_Project_Breast_Cancer_Detection.ipynb` notebook.

## Feature Engineering

Feature engineering was done to create new meaningful features and to select the most relevant ones for modeling. The details of this process are documented in the `ML_Project_Breast_Cancer_Detection.ipynb` notebook.

## Modeling

Machine learning model were trained and evaluated, including Logistic Regression.

## Model Evaluation

The models were evaluated based on accuracy, precision, recall, and F1-score. Confusion matrices and ROC curves were used to further assess model performance. The final chosen model achieved an accuracy of over 95%.

## Deployment

The final model was deployed using FastAPI, making it accessible as a web service for real-time predictions. The deployment code is available in the `app.py` file, and deployment steps are documented in the `05_deployment.ipynb` notebook.

The model was deployed on Hugging face for infinite evaluation and availability.

## Results

- **Best Model:** Logistic Regression
- **Accuracy:** 96%
- **Precision:** 97%
- **Recall:** 95%
- **F1-Score:** 96%

These results demonstrate the model's ability to accurately classify tumors as benign or malignant.



## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to customize this README to better fit your project specifics and add any additional sections you think are necessary.
