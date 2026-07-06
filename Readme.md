# Comparative Analysis of Linear Regression, Support Vector Machine, and Decision Tree for RDF-Based Mutagenicity Prediction

## Project Overview

This project predicts the mutagenicity of chemical compounds using molecular features extracted from RDF (Resource Description Framework) data. The extracted features are merged with labeled datasets and used to train and evaluate three machine learning models:

* Linear Regression (baseline classifier with thresholding)
* Support Vector Machine (SVM)
* Decision Tree

The performance of these models is compared using Accuracy, Precision, Recall, F1-score, Classification Reports, and Confusion Matrices.

---

## Project Structure

```text
.
├── Mini_Project.ipynb
├── trainingSet.tsv
├── testSet.tsv
├── mutag_stripped.nt
├── mutag_compound_features.csv
├── model_performance_comparison.csv
├── requirements.txt
└── README.md
```

---

## Requirements

Install the required Python packages using:

```bash
pip install -r Requirements.txt
```

---

## Required Libraries

* pandas
* numpy
* rdflib
* scikit-learn
* matplotlib

---

## Running the Project

Run the project using:

```bash
python Mini_Project.ipynb

```

The program performs the following tasks:

1. Loads RDF-derived molecular features.
2. Loads the training and testing datasets.
3. Merges the RDF feature matrix with the datasets.
4. Performs preprocessing and feature engineering.
5. Trains three machine learning models:

   * Linear Regression
   * Support Vector Machine (SVM)
   * Decision Tree
6. Evaluates model performance using:

   * Accuracy
   * Precision
   * Recall
   * F1-score
   * Classification Report
   * Confusion Matrix
7. Saves the output files.

---

## Input Files

* `trainingSet.tsv` – Training dataset with class labels.
* `testSet.tsv` – Testing dataset with class labels.
* `mutag_stripped.nt` – RDF representation of molecular information.
* `mutag_compound_features.csv` – RDF-derived molecular feature matrix.

---

## Output Files

* `mutag_compound_features.csv` – Extracted molecular feature matrix.
* `model_performance_comparison.csv` – Performance comparison of all machine learning models.

---

## Machine Learning Models

* Linear Regression
* Support Vector Machine (Linear Kernel)
* Decision Tree

---

## Evaluation Metrics

The following metrics are used to compare model performance:

* Accuracy
* Precision
* Recall
* F1-score
* Classification Report
* Confusion Matrix

---

## Author

Project developed as part of a machine learning assignment on prediction of carcinogenic molecule.
