# Sales_prediction
## Project Overview 
Sales Prediction is a data analysis project aimed at forecasting unit sales for a retail dataset from a Kaggle competition. The project focuses on identifying the most suitable model for predicting unit sales by analyzing historical data and exploring patterns in promotional activities. The dataset includes information from various Favorita stores located in Ecuador, with additional data on store characteristics, oil prices, and holidays.
## Dataset
The original dataset consists of several files:

**train.csv:** Contains unit sales data by date, store number, and item number. The target **unit_sales** can be integers or floats, with negative values indicating returns. The **onpromotion** column shows whether an item was on promotion, with around 16% missing values.

**stores.csv:** Metadata about stores, including city, state, type, and cluster.

**oil.csv:** Daily oil prices, relevant due to Ecuador's dependence on oil.

**holidays_events.csv:** Information on holidays and events, including transferred holidays and bridge days.

Due to the dataset's large size, this project focuses on a single randomly chosen item, using data from the last month as the test set.

## Objectives
**Model Development:** Develop models to predict unit sales using Random Forest, Gradient Boosting, and Neural Networks.

**Diagnostic Analysis:** Analyze residuals for constant variance, normality, independence, and linearity.

**Model Evaluation:** Compare the predictions with actual unit sales using Mean Squared Error (MSE) and visual plots.

## Key Findings
**Diagnostic Results:** Residuals showed no constant variance, predictors lacked a linear relationship with the response variable, and residuals were not normally distributed.

**Model Performance:** The Gradient Boosting Model (GBM) performed best, followed by Random Forest and Neural Networks.

## Limitations
The project focuses on a single item and may not generalize to other items.
There may be overfitting, and the relationship between predictors and the response variable was weak

## Usage
To run the project, clone the repository and install the dependencies:

git clone https://github.com/your-repo/sales-prediction.git

cd sales_prediction

pip install -r requirements.txt

Run the data preprocessing, model training, and prediction scripts:

## Contact
For questions or inquiries, please contact aruzhan.tuletbekova@nu.edu.kz
