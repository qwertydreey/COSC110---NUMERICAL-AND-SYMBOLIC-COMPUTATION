Activity 2: Data Cleaning and Basic Analysis
Objective:
To clean the Titanic dataset by handling missing values, fixing data types, and removing duplicates. Then, perform basic data analysis with visual insights derived from selected features.

1. Loading the Dataset
The dataset is loaded from train.csv using pandas. A preview of the data confirms the presence of missing values in the Age, Cabin, and Embarked columns, which will be addressed in the next steps.

2. Data Cleaning Process
The following cleaning steps were applied to improve data quality:

a. Standardizing Column Names
All column names were converted to lowercase and stripped of any extra spaces for consistency and easier reference.

b. Handling Missing Values
Age: Missing values were filled with the median age, a robust measure that prevents outlier distortion.

Cabin: Dropped entirely due to excessive missing entries (over 77% of rows).

Embarked: Missing values were filled with the mode (most frequent embarkation point).

These choices reflect common practices in data science:

Median is resistant to outliers.

Mode is effective for categorical imputation.

Dropping is appropriate when a column has too much missing data to be useful.

c. Visualizing Missing Values
A horizontal bar chart was generated to visually compare missing values before and after cleaning. The red bars represented missing values before cleaning; green bars represented the cleaned data. This confirmed that all targeted columns were successfully cleaned.

d. Removing Duplicates
Duplicate rows were removed to ensure data integrity.

e. Fixing Data Types
Survived and Pclass were converted to categorical for better representation.

Later, these columns were temporarily converted back to integers to support numerical analysis.

3. Saving the Cleaned Dataset
The cleaned dataset was saved locally as titanic_cleaned.csv for future use or sharing. This marks the completion of the cleaning phase.

Basic Analysis and Insights
After cleaning the dataset, two analyses were performed to derive insights from key features:

Analysis 1: Survival Rate by Passenger Class
Goal:
To determine how survival rates varied by ticket class (Pclass).

Method:
Calculated the mean survival rate within each class.

Visualized the result using a horizontal bar chart, with distinct colors for each class.

Insight:
Passengers in 1st class had significantly higher survival rates than those in 2nd or 3rd class.

This suggests that socio-economic status played a key role in survival likelihood.

Analysis 2: Age Distribution – Survivors vs. Non-Survivors
Goal:
To explore how age affected survival.

Method:
Passengers were grouped into 5-year age intervals (e.g., 0–5, 5–10, etc.).

A horizontal bar chart was created where:

Green bars represented survivors.

Red bars (in reverse direction) represented non-survivors.

Insight:
A visible cluster of survivors was seen in the young adult (20–35) age range.

Infants and young children also showed better survival rates than some older age groups.

Non-survivors were spread more evenly across age groups, though there was a notable drop in survival in the elderly.