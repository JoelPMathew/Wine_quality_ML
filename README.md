# Wine Quality ML

## Overview
This project is a **basic end-to-end machine learning pipeline** built on the classic [Wine Quality Dataset (UCI)](https://archive.ics.uci.edu/ml/datasets/wine+quality).  
It demonstrates:
- Exploratory Data Analysis (EDA)
- Preprocessing (feature scaling, label engineering)
- Supervised learning (classification & regression)
- Unsupervised learning (clustering with K-Means + PCA visualization)
- Model evaluation with accuracy, confusion matrix, and feature importance

## Project Structure

wine-quality-ml/
│── README.md          <- Project description (this file)
│── requirements.txt   <- Python dependencies
│── wine_quality.ipynb <- Main Jupyter notebook (EDA + ML pipeline)
│── figures/           <- Saved plots (EDA, confusion matrix, PCA, etc.)

## Getting Started

### 1. Clone Repository
git clone https://github.com/<your-username>/wine-quality-ml.git
cd wine-quality-ml

### 2. Install Requirements
bash
pip install -r requirements.txt

### 3. Run Notebook
jupyter notebook wine_quality.ipynb
The dataset is **loaded directly from UCI repo** (no manual download required).

## Key Features Implemented
1. EDA & Preprocessing
   - Summary statistics, correlations, histograms
   - Feature scaling with StandardScaler.
   - Binary quality label: good (≥7) vs. not good (<7)

2. Supervised ML
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - Support Vector Machine (SVM)
   - Linear Regression (predicting raw quality score)

3. Unsupervised ML
   - K-Means clustering
   - PCA for 2D visualization of clusters

4. Evaluation
   - Train/Test split
   - Accuracy & classification report
   - Confusion matrix heatmap
   - Feature importance plot


## Example Results
- Random Forest achieves ~70% accuracy on binary classification.  
- PCA + K-Means reveals rough groupings by wine quality.  
- Feature importances highlight alcohol, volatile acidity, and sulphates as key drivers.


## Tech Stack
- Python 
- pandas, numpy, matplotlib, seaborn
- scikit-learn
