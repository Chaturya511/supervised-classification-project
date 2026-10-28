# Supervised Classification Project

## Overview
This project compares Logistic Regression and Random Forest on scikit-learn's Wisconsin Breast Cancer dataset. The positive class is **malignant**.

## Files
- `supervised_classification_project.ipynb` — complete notebook with preprocessing, train/test split, 5-fold cross-validation, metrics, and plots.
- `supervised_classification_task_submission.docx` — short task report (update metrics and repository link before submitting).
- `README_supervised_classification.md` — setup and run instructions.

## Requirements
- Python 3.10 or newer
- Jupyter Notebook or JupyterLab
- pandas, numpy, matplotlib, scikit-learn

## Setup (Windows PowerShell)
```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install notebook numpy pandas matplotlib scikit-learn
```

If PowerShell blocks activation, use Command Prompt:
```bat
.venv\Scripts\activate.bat
```

## Run the notebook
From the folder containing the notebook:
```powershell
python -m notebook supervised_classification_project.ipynb
```
Or launch Jupyter and open the notebook:
```powershell
jupyter notebook
```
Then select `supervised_classification_project.ipynb` and choose **Run All**.

## Reproducibility and evaluation
- Train/test split: 80/20, stratified, random seed 42.
- Cross-validation: 5-fold StratifiedKFold on the training set.
- Algorithms: Logistic Regression and Random Forest.
- Metrics: accuracy, precision, recall, F1, ROC-AUC.
- Plots: metric comparison, confusion matrix, ROC curves.

Run every cell before submission. Copy the actual results into the report; do not invent or estimate metrics.

## GitHub upload
Create a repository on GitHub, then run these commands from the project folder:
```bash
git init
git add supervised_classification_project.ipynb README_supervised_classification.md supervised_classification_task_submission.docx
git commit -m "Add supervised classification project"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```
Replace the remote URL with your actual repository URL. If Git says a remote named `origin` already exists, use `git remote set-url origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git`.

## Important note
This is an educational project using a small curated dataset. It is not a clinical diagnostic tool.
