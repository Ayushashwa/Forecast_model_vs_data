Forecasting Models with Synthetic Data

This project explores how forecasting models behave on different dataset sizes for patient refill prediction.

We worked with two synthetic setups:

📂 Small Dataset (/kaggle/input/forecast/)

~500 patients

~2 years of data per patient (max ~3 years)

Files:

market_lookup_table.csv

prescriber_data.csv

patient_claims_data.csv

calendar_table.csv

📂 Large Dataset (/kaggle/input/forecast-exp-3/)

~5,000 patients

~9 years of data per patient (max ~11 years)

Files:

market.csv

prescribers.csv

claims.csv

calendar.csv

Data was loaded in the notebooks using:

# Example: small dataset
import pandas as pd
base_path = "/kaggle/input/forecast/"
market = pd.read_csv(base_path + "market_lookup_table.csv")
prescribers = pd.read_csv(base_path + "prescriber_data.csv")
claims = pd.read_csv(base_path + "patient_claims_data.csv")
calendar = pd.read_csv(base_path + "calendar_table.csv")


We tested three model setups on both datasets:

Baseline (0.5 threshold)

Threshold tuned (0.4)

Class-weighted model

The experiments compared accuracy, precision/recall, and patient-level refill probability distributions.
