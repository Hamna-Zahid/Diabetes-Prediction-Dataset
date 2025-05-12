
# Diabetes Prediction Dataset – Exploratory Data Analysis

## Overview

This repository contains a Jupyter notebook that performs an exploratory data analysis (EDA) on the [Diabetes Prediction Dataset](https://www.kaggle.com/datasets/mathchi/diabetes-prediction-dataset) from Kaggle. Through summary statistics and a variety of visualizations (histograms, countplots, scatterplots, and `plotnine` graphics), the notebook uncovers patterns and relationships between patient attributes (e.g., age, BMI, blood glucose, HbA1c level, gender) and diabetes outcomes.

## Dataset

- **Source**: Kaggle – _Diabetes Prediction Dataset_  
- **File**: `diabetes_prediction_dataset.csv`  
- **Description**:  
  - **Features**:  
    - `gender`  
    - `age`  
    - `hypertension`  
    - `heart_disease`  
    - `bmi`  
    - `HbA1c_level`  
    - `blood_glucose_level`  
    - `diabetes` (target: 0 = non-diabetic, 1 = diabetic)

## Contents

| File                         | Description                                |
|------------------------------|--------------------------------------------|
| `diabetes.ipynb`             | Main notebook with data loading, cleaning, summary stats, and visualizations. |
| `README.md`                  | Project overview, setup instructions, and how to use the notebook. |

## Installation & Setup

1. **Clone this repository**  
   ```bash
   git clone https://github.com/<your-username>/diabetes-eda.git
   cd diabetes-eda
   ```

2. **Create a virtual environment (optional, but recommended)**  
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Download the dataset**  
   - Register or log in to Kaggle.
   - Download `diabetes_prediction_dataset.csv` from [the dataset page](https://www.kaggle.com/datasets/mathchi/diabetes-prediction-dataset).
   - Place it under `./data/diabetes_prediction_dataset.csv` (or update the path in the notebook accordingly).

## Usage

1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `diabetes.ipynb`.
3. Run the cells sequentially to reproduce the EDA:
   - Data loading and inspection  
   - Handling missing values (if any)  
   - Summary statistics (`.describe()`, `.dtypes`)  
   - Univariate plots (`countplot`, histograms)  
   - Bivariate plots (`scatterplot`, `stripplot`, `pointplot`)  
   - Grammar of graphics with `plotnine`

## Key Findings

- **Class imbalance**: The target variable `diabetes` shows roughly equal distribution between diabetic and non-diabetic patients.
- **Age vs. Diabetes**: Older age groups tend to have a higher proportion of diabetes.
- **BMI & Blood Glucose Relationship**: Higher BMI values often correspond to elevated blood glucose.
- **HbA1c & Blood Glucose**: Clear positive trend between these two clinical markers.

*(For detailed charts and interpretations, refer to the notebook itself.)*

## Dependencies

| Library    | Version |
|------------|---------|
| Python     | ≥ 3.7   |
| pandas     | ≥ 1.2   |
| numpy      | ≥ 1.18  |
| matplotlib | ≥ 3.3   |
| seaborn    | ≥ 0.11  |
| plotnine   | ≥ 0.8   |

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for:
- Additional visualizations or modeling  
- Data‐cleaning enhancements  
- Streamlining the notebook for reproducibility

*Last updated: May 12, 2025*  
