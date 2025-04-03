# Predicting PV Output Using Weather Data

## Overview
This repository contains code and data for analyzing and predicting daily aggregate solar energy output from a photovoltaic (PV) array based on weather-related variables. The dataset spans 50 months and includes daily measurements of multiple meteorological factors. The goal is to develop a predictive model using the first two years of data for training and the last two months for evaluation.

## Dataset Description
The dataset consists of a CSV file containing the following variables:
- **precip**: Daily aggregate liquid precipitation (mm)
- **cloud cover**: Percentage of visible sky covered by clouds (%)
- **solar radiation**: Solar radiation power (W/m²)
- **humidity**: Relative humidity (%)
- **pressure**: Sea level atmospheric pressure (mbar)
- **UV index**: UV exposure level (0-10)
- **temp min**: Minimum daily temperature (°C)
- **temp max**: Maximum daily temperature (°C)
- **solar energy**: Daily aggregate solar energy (MJ/m²)
- **PV output**: Daily aggregate energy output from a 1 kWp PV array (kWh)

The goal is to use the first nine variables to predict **PV output**.

## Methodology
- **Data Preprocessing**: Cleaning and normalizing the dataset.
- **Exploratory Data Analysis (EDA)**: Understanding variable distributions and correlations.
- **Feature Selection**: Identifying key predictors for PV output.
- **Model Training**:
  - I have used XGBoost.
  - Machine learning best practices will be followed, though optimization is not required.
- **Model Evaluation**:
  - The first two years of data will be used for training.
  - The final two months of data will be used for testing and validation.
  - Performance metrics such as RMSE, MAE, and R² will be calculated.

## Implementation
- The entire implementation is carried out in **Python** within a Jupyter Notebook.
- Libraries used include:
  - `pandas` for data manipulation
  - `numpy` for numerical operations
  - `matplotlib` and `seaborn` for visualization
  - `scikit-learn` for machine learning models

## How to Use
1. Clone this repository:
   ```bash
   git clone <repo-url>
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook and follow the steps to preprocess, analyze, and train models.

## Contributions
Feel free to contribute by:
- Improving the model selection and optimization.
- Adding more advanced feature engineering techniques.
- Experimenting with additional machine learning techniques.

## License
This project is released under the MIT License.

## Contact
For any inquiries, please open an issue or submit a pull request in this repository.

