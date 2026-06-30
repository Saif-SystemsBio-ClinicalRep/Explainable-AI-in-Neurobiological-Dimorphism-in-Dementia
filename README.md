# Explainable-AI-in-Neurobiological-Dimorphism-in-Dementia
Code and models for: Mapping Neurobiological Dimorphism in Dementia Progression using Sex-Stratified Explainable AI.
## 📌 Overview
Contemporary diagnostic artificial intelligence (AI) models for Alzheimer’s disease predominantly evaluate male and female brains as a homogenous dataset. This monomorphic approach ignores inherent baseline structural dimorphism, inducing systemic algorithmic bias and clinical misclassification. 


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

This repository contains the official codebase, Jupyter notebooks, and serialized models for the research article


This repository provides a complete, reproducible computational pipeline demonstrating that neurobiological dimorphism in dementia progression cannot be mathematically reconciled within a single algorithmic architecture. By strictly stratifying clinical cohorts by biological sex and applying game-theoretic **SHAP (SHapley Additive exPlanations)** mathematics to optimized **Random Forest** ensembles, we reveal completely inverted biomarker hierarchies and map non-linear volumetric tipping points dictating dementia risk.

## 🚀 Repository Structure

* 📁 `notebooks/`: Jupyter notebooks detailing the end-to-end clinical data science pipeline.
  * `01_Data_Preprocessing_and_Imputation.ipynb`: Cohort stratification, leakage prevention, and median imputation.
  * `02_Model_Training_and_Optimization.ipynb`: GridSearchCV hyperparameter tuning, model training, and 1000-iteration bootstrapping.
  * `03_SHAP_Analysis_and_Interaction.ipynb`: XAI TreeExplainer deployment, global feature hierarchy extraction, and dependence mapping.
* 📁 `results/`: Output directories for generated figures and clinical metrics.
  * `figures/`: High-resolution visual outputs (ROC curves, SHAP Summary Plots, SHAP Dependence Plots).
  * `metrics/`: Clinical Confusion Matrices and Table 1 (Baseline Demographics).
* 📁 `models/`: Serialized `joblib` Random Forest models for external validation.
  * `rf_female_cohort_optimized.pkl`
  * `rf_male_cohort_optimized.pkl`
* 📄 `requirements.txt`: Python environment dependencies.

## 📊 Data Access (OASIS Dataset)
To ensure compliance with strict Data Use Agreements (DUA) and patient privacy standards, the raw clinical and MRI volumetric datasets are **not** hosted in this public repository. 

To reproduce this pipeline, researchers must request access to the **Open Access Series of Imaging Studies (OASIS) Cross-Sectional Dataset** directly from the official repository:
* 🔗 [OASIS Brains Official Portal](https://www.oasis-brains.org/)


## ⚙️ Installation & Requirements
To reproduce the findings, clone this repository and install the required dependencies:

```bash
# Clone the repository
git clone [https://github.com/](https://github.com/)[YourUsername]/Sex-Stratified-Dementia-XAI.git

# Navigate to the project directory
cd Sex-Stratified-Dementia-XAI

# Install required Python packages
pip install -r requirements.txt
