# Predictive Analytics Assignment 1

This repository contains the solution for Assignment 1 - Probability Density Function Parameter Estimation.

## Overview

This assignment involves:
1. Loading and cleaning air quality data (NO₂ concentrations)
2. Applying a roll-number-based non-linear transformation
3. Estimating parameters of a custom probability density function

## Files

- `Assignment-01.ipynb` - Main Jupyter notebook with complete solution
- `data.csv` - Air quality dataset containing NO₂ measurements
- Assignment PDF (if included) - Original assignment instructions

## Assignment Details

### Objective
Estimate the parameters (μ, λ, c) of the probability density function:

$$p(z) = c \cdot e^{-\lambda(z-\mu)^2}$$

### Methodology

1. **Data Loading & Cleaning**
   - Selected NO₂ feature from air quality dataset
   - Removed missing values and non-physical values (negative concentrations)

2. **Transformation**
   - Applied roll-number-based transformation: `z = x + ar·sin(br·x)`
   - Where ar and br are derived from student roll number

3. **Parameter Estimation**
   - **μ (mu)**: Mean of transformed data
   - **λ (lambda)**: Precision parameter (1/(2·variance))
   - **c**: Normalization constant (√(λ/π))

4. **Validation**
   - Visual comparison of empirical distribution vs estimated PDF

## Requirements

### Python Libraries
```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### Dependencies
- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Usage

1. Clone the repository:
```bash
git clone https://github.com/anoushkawasthi/Predictive_Assignment_1-L3-.git
cd Predictive_Assignment_1-L3-
```

2. Ensure `data.csv` is in the same directory as the notebook

3. Run the Jupyter notebook:
```bash
jupyter notebook Assignment-01.ipynb
```

## Results

The notebook estimates the three parameters of the probability density function and provides visual validation of the estimated PDF against the empirical distribution.

## Author

Anoushka Awasthi

## Date

January 2026