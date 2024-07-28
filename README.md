# sales_prediction
This project aims to forecast unit sales for Favorita stores in Ecuador using historical data, store characteristics, oil prices, and holidays. Various models, including Random Forest, GBM, and Neural Networks, were tested. The focus is on identifying the best model for accurate sales predictions. 
# Dataset
The original dataset consists of several files:

**train.csv:** Contains unit sales data by date, store number, and item number. The target **unit_sales** can be integers or floats, with negative values indicating returns. The **onpromotion** column shows whether an item was on promotion, with around 16% missing values.

**stores.csv:** Metadata about stores, including city, state, type, and cluster.

**oil.csv:** Daily oil prices, relevant due to Ecuador's dependence on oil.

**holidays_events.csv:** Information on holidays and events, including transferred holidays and bridge days.

Due to the dataset's large size, this project focuses on a single randomly chosen item, using data from the last month as the test set.

# Objectives
**Model Development:** Develop models to predict unit sales using Random Forest, Gradient Boosting, and Neural Networks.
**Diagnostic Analysis:** Analyze residuals for constant variance, normality, independence, and linearity.
**Model Evaluation:** Compare the predictions with actual unit sales using Mean Squared Error (MSE) and visual plots.

# Key Findings
**Diagnostic Results:** Residuals showed no constant variance, predictors lacked a linear relationship with the response variable, and residuals were not normally distributed.
**Model Performance:** The Gradient Boosting Model (GBM) performed best, followed by Random Forest and Neural Networks.

# Limitations
The project focuses on a single item and may not generalize to other items.
There may be overfitting, and the relationship between predictors and the response variable was weak

# Usage
To run the project, clone the repository and install the dependencies:
git clone https://github.com/your-repo/sales-prediction.git
cd sales-prediction
pip install -r requirements.txt

Run the data preprocessing, model training, and prediction scripts:

# Contact
For questions or inquiries, please contact aruzhan.tuletbekova@nu.edu.kz
