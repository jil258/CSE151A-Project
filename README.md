# CSE151A-Project --- Beer Review Prediction

## Requirements
pip install -r requirement.txt

## Introduction

In this project, we predict the overall score of the beer based on Alcohol By Volume (ABV), appearance, aroma, palate, and taste using different machine-learning models. We will begin by building up from a simple linear regression model to establish a reasonable first-pass performance baseline. Later, we used Deep Neural Network (DNN) extensively to predict overall rating and style of beers. Aside from standard analysis we learned, we also explored the usage of  PyTorch and XG Boost in Deep Learning. This repository documents our methodology, findings, and insights, providing a foundation for future research and improvements in predictive modeling for beer ratings, which could be commercialized to recommend certain types of beer to people who prefer them and offer manufactures suggestions in improving beer qualities.

## Data Exploration
Data source: [rate_beer](https://cseweb.ucsd.edu/~jmcauley/datasets.html#multi_aspect) <br>
Click on second (RateBeer) link to download ratebeer.json.gz

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

- Number of observations: 2785525
- Data distributions: left skewed
- Missing data: There is no missing data in the provided dataset
- Column descriptions: as showed aboved
  
## Data Visualization

Out dataset is the tabular data, so scatter plots will be used to visualize the relationships between different features and the target variable (average review of the overall score). 

## General workflow
### Read data from downloaded ratebeer.json.gz
### Preprocessing Steps

1. Scaling numeric features.
2. Encoding categorical features.
3. Splitting the dataset into training and testing sets.

Raw data can be found here:
[raw_data.csv](https://drive.google.com/file/d/1YE64oUNrTFDZcBJ_lK8mXtY0qImjjwyQ/view?usp=drive_link)

Cleaned data set can be found here [cleaned_numeric_data.csv](https://github.com/jil258/CSE151A-Project/blob/Milestone_3/cleaned_numeric_data.csv)

### Linear Regression
Use simple linear regression from sklearn.linear_model.LinearRegression to predict overall rating

### DNN prediction of overall rating
Use keras.layers.Dense() to create DNN model to predict overall rating using all other numeric features (ratings).

### DNN prediction of beer style
Use keras.layers.Dense() to create DNN model to predict style of beer using all numeric data.

## Running the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/jil258/CSE151A-Project.git

2. Download the data from google drive. (this step is included in the script) Preprocess and explore the data. 
3. Running Linear Regression to predict overall score using all 5 other numeric features.

## Files
1. Uncleaned and processed raw data loaded from ratebeer.json.gz dropping some not interesting columns (downloaded from source website)
[raw_data.csv](https://drive.google.com/file/d/1YE64oUNrTFDZcBJ_lK8mXtY0qImjjwyQ/view?usp=drive_link)

2. Cleaned data set can be found here [cleaned_numeric_data.csv](https://github.com/jil258/CSE151A-Project/blob/Milestone_3/cleaned_numeric_data.csv)

3. [MainModel.ipynb](https://github.com/jil258/CSE151A-Project/blob/main/MainModel.ipynb) The main file that incorporate our core workflow and model.

4. [DNN.ipynb](https://github.com/jil258/CSE151A-Project/blob/main/DNN.ipynb) Deep Neural Network prediction on overall rating using PyTorch (for extra exploration).

5. [NN_StylePrediction.ipynb](https://github.com/jil258/CSE151A-Project/blob/main/NN_StylePrediction.ipynb) Deep Neural Network to predict style of beer using other numeric features (multi-class classification)

6. [XGboost.ipynb](https://github.com/jil258/CSE151A-Project/blob/main/XGboost.ipynb) Further enhancement of [DNN.ipynb](https://github.com/jil258/CSE151A-Project/blob/main/DNN.ipynb) (Further exploration)

7. [Conclusion_section.md](https://github.com/jil258/CSE151A-Project/blob/main/Conclusion%20section.md) Conclusion section from Milestone3


## Written Report
### See this for detailed Methods, Results, Discussion, and Conclusion.
[Final Report](https://github.com/jil258/CSE151A-Project/blob/main/CSE151A_Final_Report.pdf)

## Contribution
Yang Han: Did data preprocessing and exploration, writing some part of report, improving codes, and proofreading. <br>
Leonard Shi: Help to find the dataset and abstraction. Write the Read-Me and the written report. <br>
Jian-Peng Li: Complete XGBoost training notebook, implement grid search. Complete DNN notebook,
complete corresponding section on latex file. <br>
Wen Hsin Chang: Train our first model, written report <br>
Zhaoyu Dou: Train our first model and second model. <br>
