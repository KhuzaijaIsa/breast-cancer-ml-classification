# Breast Cancer ML Classification

Machine learning classification of breast cancer clinical stage using gene expression data from the **TCGA-BRCA (The Cancer Genome Atlas – Breast Invasive Carcinoma)** dataset.

This project was developed as part of my **MSc Data Science dissertation at King's College London**.

## Project Overview

The aim of this project was to investigate machine learning methods for analysing high-dimensional biomedical data and classifying breast cancer clinical stage.

The project focuses on distinguishing **Stage III breast cancer from other stages** using RNA-Seq gene expression features.

The complete workflow includes:

- Data preprocessing and cleaning
- Integration of clinical and gene expression data
- High-dimensional feature selection
- Machine learning model development
- Cross-validation and model comparison
- Performance evaluation using multiple classification metrics

## Dataset

The project uses **TCGA-BRCA RNA-Seq gene expression and clinical data**.

The original gene expression dataset contained more than **60,000 gene identifiers**, creating a high-dimensional classification problem where the number of features was substantially larger than the number of patient samples.

Raw TCGA data are **not included in this repository**. Please refer to the official TCGA/GDC resources for information about accessing the source data.

## Methodology

### Data Preprocessing

Clinical and gene expression data were cleaned, transformed and matched by patient identifiers to create the final modelling dataset.

The classification target was defined as:

- **1:** Stage III
- **0:** Other stages

### Feature Selection

Feature selection techniques were used to reduce the very high dimensionality of the gene expression dataset before model training.

Methods investigated included:

- LASSO-based feature selection
- Statistical feature selection using t-tests

### Machine Learning Models

Several machine learning approaches were investigated and compared:

- Logistic Regression
- Random Forest
- Multi-Layer Perceptron (MLP)
- TabNet

The models were evaluated using **5-fold cross-validation**.

## Evaluation

Model performance was assessed using:

- ROC-AUC
- Precision
- Recall
- F1-score

These metrics were used to compare model performance while accounting for the characteristics of the classification problem.

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook
- Matplotlib
- Machine Learning
- Statistical Feature Selection

## Repository Structure

```text
breast-cancer-ml-classification/
│
├── notebooks/       # Data analysis and machine learning notebooks
├── src/             # Reusable Python code
├── results/         # Model evaluation results
├── figures/         # Selected visualisations
├── requirements.txt
└── README.md
```

## Academic Context

This project was completed as part of the **MSc Data Science programme at King's College London**.

The repository presents a portfolio version of the project focusing on the data science and machine learning workflow. It does not contain the raw TCGA dataset or King's College London teaching materials.

## Author

**Khuzaija Mala Isa**  
MSc Data Science, King's College London  
MSc Mathematics  
BSc Mathematics
