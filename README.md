Run the code simply on Kaggle. The Data sets can be uploaded and you can use the local library to do it.

#Use the below files for Large Datasets.

import pandas as pd
base_path = "/kaggle/input/forecast-exp-3/"
market = pd.read_csv(base_path + "market.csv")
prescribers = pd.read_csv(base_path + "prescribers.csv")
claims = pd.read_csv(base_path + "claims.csv")
calendar = pd.read_csv(base_path + "calendar.csv")

#Use the below files for Small Datasets.
import pandas as pd
base_path = "/kaggle/input/forecast/"
market = pd.read_csv(base_path + "market_lookup_table.csv")
prescribers = pd.read_csv(base_path + "prescriber_data.csv")
claims = pd.read_csv(base_path + "patient_claims_data.csv")
calendar = pd.read_csv(base_path + "calendar_table.csv")
