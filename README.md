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
The data for this project can be viewed [here](gold_price_data.csv), covering a range of financial indicators over a decade. Initial data processing involves cleaning and structuring this data for analysis, ensuring there are no missing values and that each column is formatted appropriately for the type of analysis being performed.

### **Exploratory Data Analysis**
An extensive exploratory analysis reveals underlying patterns and correlations between the different financial indicators and the price of gold. This phase helps in understanding the dynamics that affect gold prices and assists in selecting appropriate features for the prediction model.

### **Model Development and Training**
A **Random Forest Regressor** model is chosen for its efficacy in handling non-linear data and its ability to model complex interactions between inputs without extensive tuning of hyperparameters. The model is trained on a subset of the data, with careful consideration to avoid overfitting, ensuring it generalises well to new, unseen data.

### **Model Evaluation**
The performance of the model is evaluated using the **R squared metric**, which in this project, demonstrates a high degree of accuracy with a score close to 0.989. This high score indicates that the model explains nearly 99% of the variability in the response variable (gold price) around its mean, using the given predictor variables.

## **Results and Discussion**
Upon evaluating the model against the test dataset, it is evident that the Random Forest model not only fits the training data well but also accurately predicts gold prices on unseen data. Plots comparing the actual vs predicted prices illustrate the model's effectiveness, where the predicted values closely follow the actual prices, capturing both the trends and fluctuations in the gold market.

The high accuracy and reliability of the predictions demonstrate the potential of machine learning models in financial forecasting, providing valuable tools for decision-making in investments and economic analysis.

## **Conclusion**
This project exemplifies how machine learning can be applied to solve real-world problems in the financial sector. The success of the Random Forest model in predicting gold prices reaffirms the value of using advanced analytics in understanding and forecasting market dynamics.

Contributors and users of this repository are encouraged to delve into the analyses, explore further enhancements, and potentially apply the methodologies to other similar types of financial data.
