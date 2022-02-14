# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
<img width="504" alt="Screen Shot 2022-02-13 at 9 33 36 PM" src="https://user-images.githubusercontent.com/91519293/153795761-39d10d2a-2953-46b8-ba49-44deea4c87b2.png">

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Based on the summary output of the linear regression model, the variables vehicle_length and ground_clearance are statistically significant, for their corresponding p-values are less than 0.05. Both variables provided a non-random amount of variance to the mpg values in the dataset.

### Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model should not be considered to be zero because the p-value of 5.35e-11 is less than 0.05 indicating a statistical significance and we should reject our null hypothesis.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
This linear model effectively predicts mpg values of MechaCar prototypes because of the multiple R-squared value at 0.7149 which translates to 71.49% of the variability is explained by the current model.
