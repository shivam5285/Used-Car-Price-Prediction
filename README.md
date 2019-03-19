## Used-Car-Price-Prediction
### Splitting the dataset
I have splitted given dataset into train and test data in 70-30 ratio and saved those in train.csv and test.csv

### Feature Engineering
First, I have done feature engineering using heatmap plot. Unfortunately, no two features are highly correlated.
So, I have dropped only one feature 'Transaction Type' since it might not affect used car prices.

### Handling Missing Values and Labelling the data
In the given dataset, there are many rows having all fields empty except 'Price' field, so I'm dropping such rows.
Then, remaining data contains very less missing cells, so I'm dropping those too. 
Then, non-numeric values are converted to numbers using Label Encoder.

### Traning the model and predicting output
I am using Random Forest Regressor to build the model.
Then, predicted prices is saved in submission.csv for test data

### Error Calculation
I am using Mean Absolute Percentage Error to measure the error on train and test sample separately.
