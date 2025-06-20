# Laboratory Activity 1 
Computational Thinking with the Titanic Dataset using Python
*The full code and step-by-step procedures are available in the Jupyter Notebook on this folder.*

## Objectives:
1. Apply the four pillars of computational thinking: Decomposition, Pattern Recognition, Abstraction, and Algorithm Design
2. Analyze the Titanic dataset to identify key insights and stories of the data.

## Dataset:
[Check the main Titanic Dataset we used](titanic.csv)
Dataset source: [Kaggle's Dataset](https://www.kaggle.com/competitions/titanic/data)

## Key Steps:

1. Download and prepare the Titanic dataset from Kaggle.
2. Upload titanic.csv to Google Colab.
3. Load the dataset using pandas.read_csv().
4. Display the first few rows with .head() to verify successful import.

Review basic information about the dataset.

## Question Analysis:
Below is a brief overview of the questions addressed and the corresponding actions taken:

### Question No.1: Determining the underlying tasks needed to be done for loading and handling the data based on the steps described in this part.
The steps include downloading the Titanic dataset from Kaggle, renaming the file, uploading it to Google Colab, loading it with Pandas, and performing initial data inspection. This involves checking for proper loading, reviewing structure (columns and data types), identifying missing values, and deciding on any necessary cleaning.

### Question No.2: Determining the blank values in the data, using computational thinking.
After checking for nulls in each column, it was found that:

**Age** should be filled due to its importance.

**Embarked** only has two missing entries and can also be filled.

**Cabin** has too many missing values and can be removed unless a general cabin deck can be estimated using class and fare.

### Question No.3: Determining the survival rate of all passengers in the dataset, using computational thinking..
By computing the average of the Survived column (value = 0.38), the student deduce that only about 38% of passengers survived, indicating a low survival rate.

### Question No.4: Determining the average age of the survivors and non-survivors in the dataset, , using computational thinking.
It is found out that yes, the age does influenced survival:

**Young children (0–4 years)** had a higher survival rate due to prioritization.

**Middle-aged adults (15–40 years)** had lower chances, possibly due to being in social areas or unresponsive.

**Elderly passengers** had low survival due to mobility and lower priority.

