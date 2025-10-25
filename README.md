# House Sales Price Prediction - RealAgents

This repository contains code and solutions for a practical exam focused on predicting house sale prices for RealAgents, a real estate company. The goal is to optimize listing prices and reduce the time to sell by using predictive modeling techniques based on historical sales data.

## Dataset Description

The dataset contains records of house sales in one metropolitan area. It includes various features like the number of bedrooms, house type, city, area, sale price, sale date, and the number of months the house was listed. Data cleaning and preprocessing are required to handle missing values, standardize the format, and prepare the dataset for model training.

| Column Name   | Description                                                                                         |
|---------------|-----------------------------------------------------------------------------------------------------|
| house_id      | Unique identifier for houses. Missing values not possible.                                           |
| city          | The city where the house is located. One of 'Silvertown', 'Riverford', 'Teasdale', or 'Poppleton'. Missing values replaced with "Unknown". |
| sale_price    | The sale price of the house in whole dollars. Missing values removed.                                |
| sale_date     | The date of the last sale of the house. Missing values replaced with '2023-01-01'.                   |
| months_listed | Number of months the house was listed before its last sale. Missing values replaced with the mean.    |
| bedrooms      | Number of bedrooms. Missing values replaced with the mean, rounded to the nearest integer.            |
| house_type    | One of "Terraced", "Semi-detached", or "Detached". Missing values replaced with the most common type.|
| area          | Area of the house in square meters. Missing values replaced with the mean.                           |

## Tasks

### Task 1: Count Missing Cities
Calculate the number of missing values in the `city` column of the dataset.

### Task 2: Data Cleaning
Clean the dataset by replacing missing values and standardizing column formats as per the given criteria.

### Task 3: Price Analysis by Bedrooms
Produce a table showing the difference in the average sale price and variance by the number of bedrooms.

### Task 4: Baseline Model
Fit a baseline model to predict the sale price of a house using linear regression. Predictions were made on a validation set.

### Task 5: Comparison Model
Fit a more advanced model using Random Forest Regressor and compare the results with the baseline model.

## File Structure

- **`house_sales.csv`**: The original dataset containing house sales records.
- **`train.csv`**: The dataset used for training models.
- **`validation.csv`**: The dataset used for validating the model.
- **`task1.py`**: Code for counting missing cities in the dataset.
- **`task2.py`**: Code for cleaning and preparing the dataset.
- **`task3.py`**: Code for generating the price analysis by the number of bedrooms.
- **`task4.py`**: Code for fitting and predicting using the baseline model (Linear Regression).
- **`task5.py`**: Code for fitting and predicting using the comparison model (Random Forest Regressor).

## How to Use

1. Clone the repository:  
   `git clone https://github.com/subhan-0786/house-sales-prediction.git`
   
2. Install the required dependencies:  
   `pip install -r requirements.txt`
   
3. Run the tasks individually using the corresponding Python files:  
   `python task1.py`, `python task2.py`, etc.

## Results

- The Random Forest model outperformed the baseline Linear Regression model, showing better predictive accuracy on the validation set.
- Detailed analysis of house sale prices revealed that the number of bedrooms is a significant factor in determining the price.

## License

This project is licensed under the MIT License.