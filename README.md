# ICU Mortality Prediction

Predicting ICU patient mortality using clinical data and machine learning models.

## Overview

This project uses a dataset of heart failure patients to predict mortality events in the ICU.  
We explored the data, visualized feature importance, trained models, and explained predictions using SHAP values.

- **Dataset:** 299 patients, 13 features, 1 target (`DEATH_EVENT`)  
- **Target:** `DEATH_EVENT` (0 = survived, 1 = deceased)  
- **Missing data:** None  
- **Key findings:** Age, serum creatinine, and time in ICU are important features for mortality.

## Project Structure

icu-mortality-prediction/
│
├── notebooks/ # Jupyter notebooks
├── src/ # Python scripts
├── data/ # Dataset files
├── results/ # Visualizations and outputs
├── venv/ # Local virtual environment (ignored by Git)
├── requirements.txt # Python dependencies
└── README.md


## Usage

1. Clone the repository:

```bash
git clone https://github.com/berre6/icu-mortality-prediction.git
cd icu-mortality-prediction

2. Create a virtual environment and install dependencies:

python -m venv venv
venv\Scripts\activate    # Windows
pip install -r requirements.txt

3. Open the Jupyter notebooks:

jupyter notebook

Results:

-Trained models achieved around 80% accuracy.

-SHAP values used to explain the impact of features on mortality.

-Top risk-increasing features: diabetes, smoking, high_blood_pressure

-Top protective features: age, serum_creatinine, time

License:

This project is open-source and free to use.

