# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
<img width="504" alt="Screen Shot 2022-02-13 at 9 33 36 PM" src="https://user-images.githubusercontent.com/91519293/153795761-39d10d2a-2953-46b8-ba49-44deea4c87b2.png">

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Based on the summary output of the linear regression model, the variables vehicle_length and ground_clearance are statistically significant, for their corresponding p-values are less than 0.05. Both variables provided a non-random amount of variance to the mpg values in the dataset.

### Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model should not be considered to be zero because the p-value of 5.35e-11 is less than 0.05 indicating a statistical significance and we should reject our null hypothesis.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
This linear model effectively predicts mpg values of MechaCar prototypes because of the multiple R-squared value at 0.7149 which translates to 71.49% of the variability is explained by the current model.

## Summary Statistics on Suspension Coils

#### Total Lot Summary
<img width="335" alt="Screen Shot 2022-02-13 at 10 36 09 PM" src="https://user-images.githubusercontent.com/91519293/153801075-57cc2e08-f6af-46a3-8668-a8710252a5f1.png">

#### Each Lot Summary
<img width="439" alt="Screen Shot 2022-02-13 at 10 38 06 PM" src="https://user-images.githubusercontent.com/91519293/153801097-cf312870-8757-4d10-9abb-694d114beeb2.png">

### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Looking at the total lot summary, for all manufacturing lots in total, the variance of the suspensions coils do not exceed 100 pounds per square inch thus meeting the design specification. However, taking a deeper look and looking at each manufacturing lots, Lot 3 exceeds the variance target by a large margin. As a result, Lot 3 should be investigated to determine the root casue of this behavior.

## T-Tests on Suspension Coils

#### All Lots T-Test
<img width="398" alt="all_lot_t_test" src="https://user-images.githubusercontent.com/91519293/153803450-81ac2f1d-0211-433f-be43-f4e6d55f7b8e.png">
Looking at all manufacturing lots, with a p-value of 0.06028 is larger than the significane level of 0.05 meaning looking at the lots together are not statistically significant and the means are statistically similar.

#### Manufacturing Lot 1 T-Test
<img width="554" alt="lot_1_t_test" src="https://user-images.githubusercontent.com/91519293/153803469-da84d779-e01c-4a64-a215-a10b9b910f68.png">
Lot 1 T-test results show that lot 1 alone is not statistically significant becauses the returned p-value was greater than 0.05.

#### Manufacturing Lot 2 T-Test
<img width="556" alt="lot_2_t_test" src="https://user-images.githubusercontent.com/91519293/153803490-f9dea7b8-62af-4404-b7c2-507d2a4207e2.png">
Lot 2 T-test results, like the results of Lot 1 T-test, indicate that lot 2 is not statistically significant either. 

#### Manufacturing Lot 3 T-Test
<img width="558" alt="lot_3_t_test" src="https://user-images.githubusercontent.com/91519293/153803512-226e62d0-042f-4db5-9d26-35629a28752a.png">
At the other end, Lot 3 is statistically significant because the p-value of 0.04168 is lower than 0.05. With this, we can reject the null hypothesis and state that the means are not statistically similar.


