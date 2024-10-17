# **Gold Price Prediction**

## **Overview**
This repository hosts a machine learning project aimed at predicting the price of gold using historical financial data. By leveraging the **Random Forest Regression model**, this project seeks to demonstrate the applicability of machine learning techniques in financial forecasting, providing insights that could be beneficial for investors and economists alike.

## **Repository Structure**
- **Dataset**: Contains historical price data of gold and other financial indicators.
- **Jupyter Notebook**: Contains all the analyses, including data preprocessing, exploratory data analysis, model building, and evaluation.
- **Documentation**: This README file that provides an overview and guide on how to navigate and use the repository.

The core dataset includes daily recordings from the 2nd of January 2008 to the 16th of May 2018, encompassing 2290 entries. Each entry records several market indicators, including the gold price:

- **Gold price (GLD)**
- **S&P 500 index (SPX)**
- **United States Oil Fund (USO)**
- **Silver price (SLV)**
- **Euro to USD exchange rate (EUR/USD)**



This comprehensive dataset offers a detailed perspective on the market conditions that affect gold prices, establishing it as a perfect choice for predictive modeling.

## **Project Details**
### **Data Collection and Processing**
The data for this project can be viewed [here](gold_price_data.csv), covering a range of financial indicators over a decade. Initial data processing confirmed the dataset's integrity, as it contains no missing values across all entries—an essential criterion for robust data analysis. Additionally, each column is meticulously formatted to reflect its specific data type, such as floating-point numbers for financial metrics, which ensures accuracy during subsequent analytical processes.

### **Exploratory Data Analysis**

A comprehensive exploratory data analysis of the gold price dataset showed key relationships and trends amongst various financial indicators. The analysis showed that gold prices (GLD) have a strong positive correlation of 0.867 with silver prices (SLV), suggesting synchronised movements between these two precious metals. In contrast, the correlation between GLD and oil prices (USO) is -0.186, indicating a slight inverse relationship. The correlations with the S&P 500 index (SPX) and the EUR/USD exchange rate are 0.049 and -0.024, respectively, both displaying weak relationships.

### **Model Development and Training**
A **Random Forest Regressor** was chosen for this project due to its effectiveness in managing non-linear relationships and its ability to capture complex interactions between variables without the need for extensive hyperparameter tuning. The model was trained using a subset of the data, with 80% allocated for training and 20% for testing to ensure a balanced approach to learning and validation. This division helped prevent overfitting, promoting better generalisation when the model encountered new, unseen data. The Random Forest model was set up with 100 trees, leveraging the ensemble’s collective decision-making process to enhance prediction accuracy and stability. Training was conducted on the training set, followed by predictions on the test set, allowing for an evaluation of the model’s performance and its effectiveness in capturing the dynamics of gold prices.
### **Model Evaluation**
The performance of the model is evaluated using the **R squared metric**, which in this project, demonstrates a high degree of accuracy with a score close to 0.989. This high score indicates that the model explains nearly 99% of the variability in the response variable (gold price) around its mean, using the given predictor variables.

## **Results and Discussion**
Upon evaluating the model against the test dataset, the results were highly encouraging. The Random Forest model demonstrated a robust fit to the training data and achieved a notable level of accuracy in predicting gold prices on unseen data, evidenced by an R-squared error of approximately 0.989. This indicates that nearly 99% of the variance in the gold prices could be explained by the model, highlighting its predictive strength.

Graphical comparisons between the actual and predicted prices were conducted, showcasing the model’s effectiveness. The plots illustrated that the predicted values not only closely followed the actual prices but also accurately captured the trends and fluctuations inherent in the gold market.


## **Conclusion**
This project exemplifies how machine learning can be applied to solve real-world problems in the financial sector. The success of the Random Forest model in predicting gold prices reaffirms the value of using advanced analytics in understanding and forecasting market dynamics.

