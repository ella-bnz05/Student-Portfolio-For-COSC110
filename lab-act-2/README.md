# Laboratory Activity 2
Data Cleaning and Analysis using Titanic dataset <br>

*The full code and step-by-step procedures are available in the Jupyter Notebook on this folder.*

## Objectives:
1. Understand and apply fundamental data cleaning techniques using Python and Pandas.
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

### Question No.2: Deriving the data from the two basic data analysis on two columns in the dataset, and give 2 insights about it.
Passenger Age by Class:
Visualizations reveal that third-class passengers were mostly younger individuals and families, likely immigrants. Second-class included a mix of young and middle-aged professionals, while first-class passengers were generally older and wealthier, often traveling with family.

Socioeconomic Impact:
The age and class distribution highlights the link between social status and financial means. First-class passengers could afford luxury and had better access to lifeboats, increasing survival chances. In contrast, third-class passengers, often lodged in lower decks and sharing accommodations, faced more difficulty escaping, contributing to lower survival rates.

*Assisted by ChatGPT.*