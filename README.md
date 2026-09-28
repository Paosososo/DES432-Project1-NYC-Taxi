# DES432 – Project 1  
## Exploratory Data Analysis & Basic Statistical Inference  
### NYC Yellow Taxi Trip Data

---

## Dataset

Source: NYC Yellow Taxi Trip Data (Kaggle)

In the saved notebook run, the code loads the first 200,000 rows of `yellow_tripdata_2015-01.csv` (200,000 rows and 19 columns). These are the first rows of that file, not a random sample.

The notebook selects the first file in its sorted list of downloaded CSV/Parquet files. It limits CSV input to 200,000 rows; for a Parquet file, it currently loads the whole file. A future dataset version or a different selected file could therefore change the rows analyzed.

Each observation represents one taxi trip and includes time, distance, fare, passenger count, and payment information.

---

## Project Objective

This project performs exploratory data analysis (EDA) and introductory statistical inference on real-world taxi trip data.

The goals are to:

- Identify and justify data cleaning decisions
- Analyze distributional characteristics of key numerical variables
- Explore conditional patterns across groups
- Apply confidence intervals and hypothesis testing
- Interpret results under uncertainty

The focus is on statistical reasoning and interpretation rather than predictive modeling.

---

## Project Structure

The notebook is organized into the following sections:

1. Data Loading  
2. Column Detection  
3. Data Cleaning  
4. Categorical Analysis  
5. Univariate Analysis  
6. Relationship Analysis  
7. Descriptive Statistics  
8. Confidence Intervals  
9. Hypothesis Testing  
10. Bayesian Conditional Probability Analysis  

---

## Key Cleaning Decisions

- Removed negative fare_amount values
- Removed trips with passenger_count = 0
- Retained plausible long-distance trips (under 100 miles)
- Preserved missing tip_amount values
- Grouped missing RatecodeID as "Unknown"

---

## How to Run

1. Open the notebook in Google Colab.
2. Run all cells from top to bottom.
3. The dataset is automatically downloaded using `kagglehub`.
4. No manual dataset upload is required.

Required libraries:
- pandas
- numpy
- seaborn
- matplotlib
- scipy
- kagglehub

---

## Reproducibility

All results, figures, and summary statistics in the report are generated directly from the notebook.

The notebook is designed to run sequentially without modification.
