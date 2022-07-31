# IIT_Kaatru_assignment

# ASSIGNMENT- KAATRU  IIT MADRAS


## Goal:
Develop a model to find the variables that are significant in the demand for shared bikes with
the available independent variables and report appropriate metrics of your model evaluation.



## Outcome:

The variables that are significant in predicting the demand for shared bikes (at least 3).


## Note: 
cnt is the dependent variable



### instructions to Run the code for Assignment 


 - [Required Data(google drive link) ](https://drive.google.com/drive/folders/1-M64d6-cWzQgiG7vxSfu-QN3EdBYw9PT?usp=sharing)
 - [Jupyter notebook (contains other approaches i tried)](https://github.com/ravipratap366/IIT_Kaatru_assignment/blob/main/assignment-iit_kaatru%20(1).ipynb




## summary
#### approaches i tried
-  Filter Method: 
 In this method, features are dropped based on their relation 
 to the output, or how they are correlating to the output. I use 
 correlation to check if the features are positively or negatively 
 correlated to the output labels and drop features accordingly.


-  Wrapper Method: 
We split our data into subsets and train a model using this.
 Based on the output of the model, we add and subtract features and 
 train the model again. It forms the subsets using a greedy approach
  and evaluates the accuracy of all the possible combinations of 
  features. Eg: Forward Selection, Backwards Elimination,
  Recursive Feature Elimination etc.

  top 3 by RFE selected variables are -- yr,temp and weathersit


- Intrinsic Method: 
This method combines the qualities of both the Filter and Wrapper 
method to create the best subset.

This method takes care of the machine training iterative process 
while maintaining the computation cost to be minimum.
 Eg: Lasso and Ridge Regression.

  top 3 by rf.feature_importances_ variables  are  --  temp,year and season



- Variance Inflation Factor (VIF)
Variance inflation factor (VIF) is a measure of the amount of 
multicollinearity in a set of multiple regression variables. 
Mathematically, the VIF for a regression model variable is equal
 to the ratio of the overall model variance to the variance of a 
 model that includes only that single independent variable. 
 This ratio is calculated for each independent variable. A high VIF 
 indicates that the associated independent variable is highly collinear
  with the other variables in the model.



### final report
As per our final Model, the top 3 predictor variables that influences the bike booking are: 
- **Temperature (temp)** 
- **weathersit_3** 

- **Year (yr)**








