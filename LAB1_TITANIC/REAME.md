Activity 1: Data Loading and Basic Exploration of the Titanic Dataset
Objective:
To load the Titanic dataset, perform initial data inspection, and identify any missing or blank values. This step is essential before performing further data analysis or model building.

1. Uploading the Dataset
The activity begins by prompting the user to upload the Titanic dataset using Google Colab's file upload feature. Once uploaded, the script confirms the file is present in the working directory.

Key Tasks:

Import required libraries like os, files from google.colab, and matplotlib.pyplot.

Upload the titanic.csv file interactively.

Check and print the working directory to ensure the file was uploaded successfully.

2. Reading the Dataset
Using pandas, the CSV file is read into a DataFrame for manipulation. A preview of the first five rows is displayed using tabulate() to present the data in a readable table format.

Initial Columns Observed:

PassengerId, Survived, Pclass, Name, Sex, Age

SibSp, Parch, Ticket, Fare, Cabin, Embarked

From the preview, it's immediately visible that several rows have missing values in the Cabin and Age columns.

3. Dataset Information Overview
The script uses the .info() method from pandas to generate a summary of the dataset, including:

Total number of entries (891)

Number of columns (12)

Data types of each column

Number of non-null values per column

Memory usage

This provides insight into the structure and completeness of the data.

4. Statistical Summary
Using .describe(), the activity computes basic statistical summaries for numeric columns:

Count, Mean, Standard Deviation

Minimum and Maximum values

25th, 50th (Median), and 75th percentiles

This helps identify ranges, outliers, and distributions of numerical features like age and fare.

5. Missing Value Detection
The number of missing values per column is calculated using isnull().sum(). The results are filtered to show only those columns with missing data:

Missing Values Found In:

Age: 177 missing values

Cabin: 687 missing values

Embarked: 2 missing values

This step is crucial to prepare for data cleaning or imputation in future activities.