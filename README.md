# MSCS 5622 Supervised Learning Project
### Authored by Sean Norman
#### April 2025

## Executive Summary
Analyze the relationship between Consumer Price Index (CPI) and revolving consumer credit volume using monthly data from 2019 through early 2025 for exploratory data analysis (EDA) and model training, and test predictive models on subsequent monthly data (January–March 2025). This analysis would be useful in better understanding when revolving consumer credit volume is expected to bloom as a result of the CPI trends. If this could be determined it may inform personal actions that could be taken to prevent investment risk or capitalize on opportunities.

**Data Source Reference**:
*   U.S. Bureau of Labor Statistics. (2025). *Consumer Price Index for All Urban Consumers (CPI-U): U.S. city average, All series [CUUR0000+]*. Retrieved from https://data.bls.gov/dataViewer/view/timeseries/CUUR0000SA0
*   Federal Reserve Bank of St. Louis. (2025). *Consumer Credit Outstanding (Levels), Revolving [REVOLNS]*. Retrieved from https://fred.stlouisfed.org/series/REVOLNS

### Report Summary (Notebook is the Report)
Comments are included in all code cells to explain the thought process and intent of what the code is doing.

At the end of the notebook is a report summary that addresses the approach along with discussion around learnings, takeaways, suggestions, and future considerations for next steps. Please review these details to better understand the conclusion of this exercise.

### Learning & Algorithms Utilized
In this analysis the following modeling was performed:
- Linear Regression
- Random Forest
- Random Forest w/ Hyperparameter Tuning
- XGBoost (Gradient Boost)
- XGBoost (Gradient Boost) w/ Hyperparameter Tuning

## About this repository
In this repository you will find the following materials:

```
├── data/
├── .venv/                  # Python virtual environment (created by setup scripts)
├── environment-config.md   # Instructions for setting up the Python environment
├── ml-notebook.html        # Main Jupyter notebook as HTML for report viewing
├── ml-notebook.ipynb       # Main Jupyter notebook for analysis
├── README.md               # This file
├── requirements.txt        # List of Python package dependencies
├── setup.bat               # Setup script for Windows (note: this is included and was generated from the setup.sh file and has not been tested.)
├── setup.sh                # Setup script for macOS/Linux
```

### `data/` folder
This folder contains the raw data sourced as noted in the ml-notebook file

### `model-notebook.ipynb`
This is a Jupyter notebook that contains all of the work from loading, to cleaning data and on through EDA, analysis, model definition, model training, and model testing. Various outputs are created as a result of running this notebook and those are stored in the output directory.

### Environment Setup Files
*   **`environment-config.md`**: Contains detailed instructions on how to set up the necessary Python virtual environment using the provided scripts.
*   **`requirements.txt`**: Lists the specific Python packages and versions required to run the notebook.
*   **`setup.sh`**: A shell script for macOS and Linux users to automate the creation of the virtual environment and installation of dependencies.
*   **`setup.bat`**: A batch script for Windows users to automate the creation of the virtual environment and installation of dependencies.

## Disclosure & Responsible Use
The data used in this project was obtained via public government sites and is considered to be an open dataset. The analysis performed in this project is original work and intended for educational purposes only. The project is an assignment that is part of Machine Learning class work and should not be copied by any student. It is shared here to support the required deliverable for the project.