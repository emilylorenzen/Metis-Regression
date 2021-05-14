Linear Regression Module - Minimal Viable Project

Emily Lorenzen

# Modeling the percent difference between sold and listed prices for recently sold homes in Portland, OR

To formulate a linear regression model, I used percent difference between sold and listed home prices as the target variable and the top 5 features which showed the largest absolute correlation with the target. These features were number of favorites on redfin, price per square foot, hoa dues, and walk score. The evaluation metrics for the training data are displayed below. 

![image](https://user-images.githubusercontent.com/25285730/117883767-ac2a7400-b260-11eb-8b55-1fcc8dfda0d3.png)

For the validation data here is how the model performed: 

Validation R^2 score was: 0.156105903965164
Feature coefficient results: 

favorites_redfin : 2.4414187692790548
lot_size : 0.8152377879681012
price_sq_ft : 1.3958074025022087
hoa_dues : -1.415598791822415

![image](https://user-images.githubusercontent.com/25285730/117884423-75a12900-b261-11eb-9fba-81ec39a385c2.png)

A jointplot of predicted values vs. actual values reveals a lot to be desired in this model. 

![image](https://user-images.githubusercontent.com/25285730/117884544-9cf7f600-b261-11eb-948e-6380f0c734b6.png)

Finally, the diagnostic plots show that the residuals are heavy-tailed. 
