# College Football Playoff (CFP) Prediction Project
## 👥 Project Team

- **Evan Mansfield** – Project Lead

<img width="360" alt="Screenshot 2025-05-12 at 4 51 21 PM" src="https://github.com/user-attachments/assets/4069f43c-ff50-453c-9831-608c6701cf93" />

- **Robert Villavicencio** – Data Scientist/Engineer
  
  <img width="360" alt="Screenshot 2025-05-12 at 4 47 57 PM" src="https://github.com/user-attachments/assets/7dd6432c-b60d-422a-bf02-1285b4fbabbe" />

- **Samantha Barry** – Project Analyst  
- **Charlotte Finnerty** – Project Analyst  

  

This project aims to predict the College Football Playoff Bracket for the 2024 season using historical data and machine learning models. The project utilizes various data scraping techniques, data preprocessing methods, and machine learning models to make accurate predictions.

## Table of Contents

- [Introduction](#introduction)
- [Data Sources](#data-sources)
- [Setup and Installation](#setup-and-installation)
- [Notebook Overview](#notebook-overview)
- [Results](#results)
- [Challenges and Limitations](#challenges-and-limitations)
- [Contributors](#contributors)
- [License](#license)

## Introduction

The goal of this project is to predict which teams will be selected for the College Football Playoff bracket for the 2024 season. The project uses historical data, team statistics, and various machine learning models to make predictions.

## Data Sources

The data used in this project includes:
- Historical College Football Playoff (CFP) rankings
- Team statistics from 2014 to 2023
- Game results and scores
- Web scraping from Sports Reference and other relevant websites

## Setup and Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/EvanMansfield/CFP_Prediction_FinalProject.git
    cd CFP_Prediction_FinalProject
    ```

2. Set up a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Open the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

5. Navigate to the `CFP_Prediction_Project.ipynb` file and run the cells in sequence.

## Notebook Overview

### Google Drive Integration
- **Mounting Drive:** Uses `google.colab.drive` to access Google Drive files for reading and writing directly within Google Drive.

### Data Packages and Functions
- **Packages Installed:**
  - `pandas`, `numpy` for data manipulation.
  - `scikit-learn` for machine learning (Logistic Regression, StandardScaler, LabelEncoder).
  - `xgboost` for XGBoost classification.
  - `matplotlib`, `seaborn` for data visualization.
  - `requests`, `beautifulsoup4`, and `lxml` for web scraping.
  - `urllib3` for secure HTTP requests.

### Web Scraping
- Extracts College Football data from Sports Reference using `requests` and `BeautifulSoup`.
- Saves the output as CSV files.

### Data Preprocessing
- Handles missing values using `SimpleImputer`.
- Standardizes numeric features using `StandardScaler`.
- Encodes categorical columns using `LabelEncoder`.

### Machine Learning Models
1. **Logistic Regression Model:**
   - Predicts whether a team makes the College Football Playoff based on key performance metrics.
   - Outputs probabilities, accuracy scores, and a classification report.

2. **XGBoost Model:**
   - Trains an XGBoost Classifier to predict playoff chances.
   - Provides better handling of large datasets and missing values.
   - Outputs playoff probabilities and compares performances.

### Visualization
- Creates line plots and bar graphs showing playoff probabilities.
- Displays team names, AP rankings, and conference groupings.

## Results

The predictions and results will be displayed within the notebook. The final predictions for the CFP bracket, along with various visualizations and metrics used to evaluate the model's performance, will be shown.

## Challenges and Limitations

- **Website Blocking:** Multiple rapid scraping attempts may be blocked or limited by the website.
- **Cost of Accurate Data:** Premium data access from verified providers might be required for full accuracy and real-time data.
- **Alternative Solutions:** Implementing a staggered scraping approach over time to avoid detection and blocking.

