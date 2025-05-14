# Smart Property Price Predictor

Final project for the Building AI course

## Summary

This project uses machine learning to predict real estate property prices based on features such as area, number of rooms, location, and condition. It helps buyers and sellers make data-driven decisions in the housing market.

## Background

Property price estimation is often subjective and inconsistent. Real estate markets are dynamic, and individuals often rely on intuition or outdated comparisons when estimating prices. This leads to overpricing, underpricing, and frustration for buyers and sellers alike.

This project aims to:
* Predict accurate prices for homes using AI
* Assist users in understanding the key price-driving factors
* Reduce the risk of pricing errors in property listings

Personal motivation: I’ve often seen friends struggle to price their properties realistically, leading to financial or emotional loss. AI can assist by making this process objective.

## How is it used?

The solution is used via a web or mobile app where the user inputs property features:
* Area (in square meters or feet)
* Number of bedrooms and bathrooms
* Location (city/zip code)
* Year built
* Additional features (e.g. garage, garden)

The model then predicts the expected price instantly.

Target users:
* Homeowners looking to sell
* Real estate agents
* Property investors
* First-time buyers comparing values

<img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/Real_estate_graph.jpg" width="400">

## Data sources and AI methods

Data:
* Public housing datasets from [Kaggle](https://www.kaggle.com/datasets)
* Local real estate listing sites (via web scraping or open APIs)

AI techniques:
* Regression using neural networks
* Feature scaling and normalization
* Evaluation using MAE, RMSE

Example implementation:
```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X_train, y_train)
prediction = model.predict(X_test)
