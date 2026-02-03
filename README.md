# Project-Exploring-NYC-Public-School-Result-Scores

# NYC SAT Results Analysis

This project analyzes SAT performance across New York City public schools using Python and pandas.  
The objective is to evaluate academic performance at both the **school level** and the **borough level** through descriptive statistics and data aggregation.


##  Dataset
The dataset contains SAT performance data for NYC schools, including:
- `school_name`
- `borough`
- `average_math`
- `average_reading`
- `average_writing`

---

## Objectives
- Identify NYC schools with the best math results.
- Rank schools based on combined SAT scores.
- Determine which borough has the largest variability in SAT performance.

---

##  Methodology

### Best Math Performing Schools
- Defined strong math performance as scores **≥ 80% of the maximum SAT math score (640 out of 800)**.
- Filtered schools meeting this criterion.
- Selected relevant columns and sorted results in descending order.

### Top Performing Schools by Combined SAT Score
- Created a new metric `total_SAT` as the sum of math, reading, and writing scores.
- Ranked schools by `total_SAT` and selected the top 10 performers.

### Borough-Level Statistical Analysis
- Calculated `total_SAT` for all schools.
- Grouped data by borough to compute:
  - Number of schools (`num_schools`)
  - Mean combined SAT score (`average_SAT`)
  - Standard deviation of combined SAT score (`std_SAT`)
- Identified the borough with the **largest standard deviation**, indicating the greatest variability in school performance.
- Rounded all numeric values to two decimal places.

---

## Visualization
A bar chart was generated to visualize the **standard deviation of combined SAT scores by borough**, enabling clear comparison of performance variability across NYC boroughs.


