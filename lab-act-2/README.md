# Laboratory Activity 1 
Data Cleaning and Analysis using Titanic dataset <br>

*The full code and step-by-step procedures are available in the Jupyter Notebook on this folder.*

## Objectives:
1.  Understand and apply fundamental data cleaning techniques using Python and Pandas.
2. Learn how to handle missing values, remove duplicates, convert data types, and more.
3. Use the cleaned dataset for basic data analysis

## Dataset:
Check the dataset that I used: [Local dataset file](titanic.csv) <br>
Dataset source: [Kaggle's Dataset](https://www.kaggle.com/competitions/titanic/data)

## Key Steps in the Activity:

1. Load and understand the dataset.
2. Drop irrelevant columns.
3. Handle missing values.
4. Convert numerical columns such as Survived and Pclass to categorical for efficiency.
5. Remove duplicates.
6. Standardize column names.
7. Review basic information about the dataset.

## Question Analysis:
Below is a brief overview of the questions addressed and the corresponding actions taken:

### Question No.1: Reason for the used algorithm  or key steps in cleaning the dataset. 

This algorithm was utilized to handle missing values, remove unnecessary data, and improve the dataset for analysis.

By understanding the data, you can identify important aspects such as data types, missing values, and potential issues before cleaning. Removing the PassengerId column is necessary since it is unique and does not contribute to the analysis.

Using the median for missing ages ensures that the estimated values are more representative of most passengers' age. Handling missing Cabin values can help analyze which parts of the Titanic had the highest survival rates. However, if estimating the cabin locations is not feasible, the column can be dropped. For missing Embarked values, only two entries are missing, so replacing them with the mode, most frequent value, is a reasonable approach.

Converting Survived and Pclass into categorical data saves memory and improves processing speed. Checking for duplicate entries and removing is part of cleaning the data and prevents biases in analysis. Standardizing column names helps avoid confusion when analyzing and visualizing data. Lastly, saving the data is necessary for further analysis.

### Question No.2: Determining the blank values in the data using computational thinking.
After checking for nulls in each column, it was found that:

**Age** should be filled due to its importance.

**Embarked** only has two missing entries and can also be filled.

**Cabin** has too many missing values and can be removed unless a general cabin deck can be estimated using class and fare.

### Question No.3: Determining the survival rate of all passengers in the dataset using computational thinking..
By computing the average of the Survived column (value = 0.38), I deduced that only about 38% of passengers survived, indicating a low survival rate.

### Question No.4: Determining the average age of the survivors and non-survivors in the dataset using computational thinking.
It is found out that yes, the age does influenced survival:

**Young children (0–4 years)** had a higher survival rate due to prioritization.

**Middle-aged adults (15–40 years)** had lower chances, possibly due to being in social areas or unresponsive.

**Elderly passengers** had low survival due to mobility and lower priority.

