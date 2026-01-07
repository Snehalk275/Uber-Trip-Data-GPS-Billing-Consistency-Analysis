🚕 NYC Yellow Taxi trip records (NYC TLC) – GPS & Billing Consistency Analysis

This project analyzes NYC Yellow Taxi trip data published by the NYC Taxi & Limousine Commission to identify inconsistencies between GPS-recorded distance and customer billing.
The goal is to understand how missing or incorrect telemetry (GPS data) can impact revenue reporting, customer billing, and operational metrics.

📂 Dataset
Source: NYC Taxi & Limousine Commission (TLC)(yellow_tripdata_2025-01)

The data contains real trip records including:
Pickup & drop-off locations
Trip distance
Fare & total amount
Payment type
Timestamps
This is regulatory data submitted by transportation providers.

🔍 Problem
While exploring the data, some trips were recorded with zero travel distance but still had non-zero fare and total charges.
This suggests that the ride was completed and billed, but GPS distance data was missing or not captured correctly.

📊 Key Findings
Metric	Value
Zero-distance trips	~90,893
Share of all trips	~2.62%
Revenue from zero-distance trips	~$2.12M
Share of total revenue	~2.39%
Maximum single fare	$950
Fare ↔ Total correlation	0.98
Revenue was also concentrated in specific pickup zones, indicating systematic GPS or telemetry gaps rather than random noise.

📈 Analysis Performed

The project includes:
Exploratory Data Analysis (EDA)
Distribution of trip distance and fares
Distance vs fare visualization
Zero-distance trip analysis
Revenue impact calculation
Pickup zone concentration analysis

🧠 Why this matters
This type of analysis helps organizations:
Validate billing accuracy
Monitor data quality
Identify telemetry gaps
Assess revenue integrity
Support compliance & reporting

🛠 Tools Used
Python
Pandas
Parquet
Matplotlib
Exploratory Data Analysis
