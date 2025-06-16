# BayesianModelling

This repository contains a collection of Jupyter notebooks focused on Bayesian modeling techniques, with applications to real-world datasets. The main tools used are [PyMC](https://www.pymc.io/), [ArviZ](https://python.arviz.org/), and standard scientific Python libraries.

## Contents

### 1. `analytical_approximation.ipynb`
- **Purpose:**  
  Explores analytical and variational approximations in Bayesian model selection, focusing on polynomial regression.
- **Key Topics:**  
  - Fitting polynomials of various degrees to a dataset.
  - Model evidence (marginal likelihood) and its role in Bayesian model selection.
  - Laplace approximation and ADVI (Automatic Differentiation Variational Inference) for estimating model evidence.
  - Mathematical explanations and practical code for both approaches.
- **Key Outcomes:**  
  Use function-fitting algorithms to estimate model evidence, and compare the strengths and weaknesses of Laplace and ADVI methods.

### 2. `UK_GP_Visit_Estimations.ipynb`
- **Purpose:**  
  Bayesian modeling of healthcare data: estimating the number of General Practitioner (GP) visits in the UK, stratified by region and age group, with missing data imputation.
- **Key Topics:**  
  - Data cleaning and preprocessing of a 3D array (region × age group × samples).
  - Zero-Inflated Poisson models to account for excess zeros in count data.
  - Hierarchical (partial pooling) vs. complete pooling Bayesian models.
  - Model comparison, cross-validation, and visualization of predictions.
- **Key Outcomes:**  
  Build and compare hierarchical Bayesian models for count data, handle missing values, and interpret model predictions in a real-world context.

### 3. `SF_weather_prediction.ipynb`
- **Purpose:**  
  Focuses on Bayesian regression modeling for weather prediction in San Francisco using different likelihood functions.
- **Key Topics:**  
  - Probabilistic modeling of weather data.
  - Application of Bayesian inference to regression problems.
- **Key Outcomes:**  
  Apply Bayesian methods to environmental data and interpret probabilistic forecasts.

### 4. `sf.csv`
- **Purpose:**  
  Data file,  used in `SF_weather_prediction.ipynb` for weather modeling.

---

## Getting Started

1. **Install dependencies:**  
   Most notebooks use PyMC, ArviZ, NumPy, pandas, and Matplotlib.  
   You can install the main dependencies with:
   ```bash
   pip install pymc arviz numpy pandas matplotlib
   ```

2. **Open the notebooks:**  
   Use JupyterLab or Jupyter Notebook to explore and run the code interactively.

---

## Project Highlights

- Demonstrates practical Bayesian modeling on real datasets.
- Compares different inference and approximation techniques.
- Includes both code and detailed mathematical explanations.