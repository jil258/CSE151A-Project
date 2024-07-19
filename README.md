# CSE151A-Project

## Requirements
pip install -r requirement.txt

## Beer Review Prediction

This project aims to predict the average review/overall score of each specific beer based on various features. The dataset contains information about different beers, including their ABV, style, and review scores in different aspects.

Our analysis is done through [data_exploration.ipynb](https://github.com/jil258/CSE151A-Project/blob/Milestone_3/data_exploration.ipynb)


## Data Exploration

The dataset contains the following columns:

- `beer/beerId`: Unique identifier for each beer.
- `beer/ABV`: Alcohol by volume of the beer.
- `beer/style`: Style of the beer. (string)
- `review/appearance`: Appearance review score (out of 5).
- `review/aroma`: Aroma review score (out of 10).
- `review/palate`: Palate review score (out of 5).
- `review/taste`: Taste review score (out of 10).
- `review/overall`: Overall review score (out of 20).

## Data Description

- Number of observations: 
- Data distributions: [Describe the distributions, e.g., normal, skewed]
- Scales: [Specify if any columns need scaling]
- Missing data: There is no missing data in the provided dataset
- Column descriptions: [Provide a brief description of each column]

## Data Visualization

Out dataset is the tabular data, soscatter plots will be used to visualize the relationships between different features and the target variable (average review of the overall score). 

## Preprocessing Steps

1. Scaling numeric features.
2. Encoding categorical features.
3. Splitting the dataset into training and testing sets.
4. Finding the average review of the overall score for each identical beerID in testing sets.

The details of the above steps will be provided in the Jupyter Notebook.

Raw data can be found here:
[raw_data.csv](https://drive.google.com/file/d/1YE64oUNrTFDZcBJ_lK8mXtY0qImjjwyQ/view?usp=drive_link)

Cleaned data set can be found here [cleaned_numeric_data.csv](https://github.com/jil258/CSE151A-Project/blob/Milestone_3/cleaned_numeric_data.csv)

### Running the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/jil258/CSE151A-Project.git

2. Download the data from google drive. (this step is included in the script) Preprocess and explore the data. 
3. Running Linear Regression to predict overall score using all 5 other numeric features.

### Recent update from Milestone 2
We did linear regression to predict overall rating using other 5 numeric features (ABV, appearance, aroma, palate, taste)
