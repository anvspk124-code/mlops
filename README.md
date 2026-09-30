# 🌍 Earthquake Magnitude Prediction

A machine learning project for predicting **earthquake magnitude** from earthquake-related data. The project follows a structured and reproducible ML workflow including **data validation, preprocessing, model training, evaluation, experiment tracking, and model management using MLflow**.

## 📌 Project Overview

Earthquake magnitude prediction is a regression problem where the goal is to predict the magnitude of an earthquake based on available earthquake-related features.

This project implements an end-to-end machine learning pipeline:

```text
Raw Dataset
     ↓
Data Validation
     ↓
Data Preprocessing
     ↓
Feature Engineering
     ↓
Model Training
     ↓
Model Evaluation
     ↓
MLflow Experiment Tracking
     ↓
Model Registration
```

## 🎯 Objectives

- Validate the input earthquake dataset.
- Clean and preprocess the data.
- Prepare features for machine learning.
- Train regression models.
- Evaluate model performance using MAE, RMSE, and R².
- Track experiments using MLflow.
- Register trained models for model version management.
- Maintain a reproducible machine learning workflow.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- MLflow
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git & GitHub

## 📂 Project Structure

```text
Earthquake_Magnitude_Prediction/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── project_implementation.ipynb
│
├── src/
│   ├── data_validation.py
│   ├── preprocessing.py
│   ├── train.py
│   ├── evaluate.py
│   └── ...
│
├── models/
│
├── README.md
├── requirements.txt
└── .gitignore
```

## 🔄 Machine Learning Workflow

### 1. Data Validation

The dataset is checked for:

- Missing values
- Duplicate records
- Invalid data types
- Required columns
- Invalid or inconsistent values

### 2. Data Preprocessing

The data is prepared for model training through:

- Missing-value handling
- Feature selection
- Encoding categorical features where required
- Numerical feature processing
- Train-test splitting
- Feature transformation

### 3. Model Training

Regression models are trained using the processed dataset.

The trained models are evaluated on unseen test data.

### 4. Model Evaluation

The following regression metrics are used:

| Metric | Description | Better |
|---|---|---|
| MAE | Average absolute prediction error | Lower |
| RMSE | Penalizes larger prediction errors | Lower |
| R² | Variance explained by the model | Higher |

### 5. Experiment Tracking with MLflow

MLflow is used to track machine learning experiments.

The following information can be recorded:

- Parameters
- Metrics
- Trained models
- Plots
- Reports
- Other experiment artifacts

Example:

```text
Experiment
│
├── Parameters
├── Metrics
├── Model
└── Artifacts
```

### 6. Model Registration

The trained model can be registered in the MLflow Model Registry.

This allows different model versions to be managed and retrieved for deployment.

## 📊 Model Performance

Model performance is evaluated using:

```text
MAE
RMSE
R² Score
```

The best-performing model is selected based on the evaluation results and project requirements.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Earthquake_Magnitude_Prediction.git
```

### 2. Navigate to the project

```bash
cd Earthquake_Magnitude_Prediction
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

### 4. Activate the environment

Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the training pipeline

```bash
python src/train.py
```

### 7. Start MLflow

```bash
mlflow ui
```

Then open the MLflow interface in your browser.

## 📈 MLflow

MLflow is used for:

- Experiment tracking
- Parameter logging
- Metric logging
- Artifact logging
- Model logging
- Model registration

This makes the machine learning workflow more reproducible and easier to compare.

## 🔬 Future Improvements

- Hyperparameter optimization
- Advanced regression models
- Automated data validation
- Model monitoring
- Model drift detection
- Automated CI/CD pipeline
- Cloud deployment
- Streamlit-based prediction interface

## 👨‍💻 Author

**Pavan**

Machine Learning / AI Project
