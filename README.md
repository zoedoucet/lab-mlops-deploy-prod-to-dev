# -lab-mlops-deploy-prod-to-dev
# Churn Prediction – MLOps Lab

## Project Description

This project trains a machine learning model to predict customer churn using a telecom dataset.

The goal of this lab is to practice the MLOps workflow, including virtual environments, dependency management, model validation, Git branches, pull requests, and code reviews.

## Requirements

- Python 3.12 (or your installed version)
- pandas
- scikit-learn
- joblib

## Setup

Create and activate a virtual environment:

```bash
python -m venv .venv
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the Model

Train and save the model:

```bash
python train.py
```

Validate the model:

```bash
python check_model.py
```

The model must achieve a test ROC AUC of at least **0.80** to pass validation.

## MLOps Workflow

1. Develop on a separate Git branch.
2. Push changes and create a pull request.
3. Review and test the model.
4. Merge into `main` only after validation passes.

The trained model and virtual environment are excluded from Git using `.gitignore`.