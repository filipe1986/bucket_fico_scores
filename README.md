# J.P. Morgan Forage - Task4: FICO Score Bucketing

## Objetive
Convert continuous FICO scores (300-850) into categorical buckets to be used as input for a machine learning model.

## Approach
I used **Quantile-based bucketing** (`pd.qcut`) to create 8 balanced buckets based on the data distribution.

## Key Files
-`fico_score.ipynb`  → Main notebook with analysis and bucketing
-`fico_buckets.csv`  → Dataset with added bucket columns
-`loan_data.csv`  → Original data

## Results
- Successfully created 8 FICO buckets
- Each bucket has a meaningful label (e.g. "Poor", "Fair", "Good", etc.)
- Default rate varies significantly across buckets (as expected)

## Method Used
Quantile discretization using pandas `qcut()`. This ensures each bucket has approximately the same number of observations.

## Next Steps
This bucketing can now be used as a categorical feature for the Probability of Default model.

---
Submitted by Filipe Vieira
