# CSE151A-Project

install pip install gdown
https://drive.google.com/file/d/1YE64oUNrTFDZcBJ_lK8mXtY0qImjjwyQ/view?usp=drive_link

# Beer Review Prediction

This project aims to predict the average review/overall score of each specific beer based on various features. The dataset contains information about different beers, including their ABV, style, and review scores in different aspects.


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

### Running the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/jil258/CSE151A-Project.git
