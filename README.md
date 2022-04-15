# MechaCar_Statistical_Analysis

## Project Overview:

 AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has hired the new employee (Jeremy) and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, Jermy and the data analytics team do the following:

1) Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
2) Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
3) Run t-tests to determine if the manufacturing lots are statistically different from the mean population
4) Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, write a summary interpretation of the findings.

## Linear Regression to Predict MPG:

![Summary 1](https://user-images.githubusercontent.com/96403349/163402180-632abcf5-40bb-4b55-8421-409f4042edbd.png)

1) The above screenshot we can see the the results of producing a linear regression model to predict MPG from the MechaCar_mpg dataset by using the variables of vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD. So the vehicle length, and ground clearance are statistically likely to provide non-random amounts of variance to the model which significant impact on miles per gallon on the MechaCar prototype. However, the vehicle weight, spoiler angle, and AWD ( All Wheel Drive) have p-Values that indicate a random amount of variance with the dataset.

2)  The slope of the linear model is not considered to be zero because the estimates for all coefficients are not zero. This is because, p-value is 5.35e-11 which much smaller than the significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, and slope of this linear model is non zero. 

3) This linear model predicts the mpg of MechaCar protoypes effectively because the Adjusted R-squared reflects that 0.7149, which means that approximately 71% of the variation within mpg is explained by the coefficients.

## Summary Statistics on Suspension Coils:

The Suspension Coil dataset provided for the MechaCar contains the results show that the variance of the suspension coils is 62.29 which must not exceed 100 pounds per square inch (PSI) when we looking the entire pouplation of the production lot. However, lot summary shows that Lot 1 and Lot 2 are well within the 100 PSI variance requirement with variances of 0.98 and 7.47 respectively. On the other side, lot 3 does not meet the design specifications as its variance is 170.29 which much over the 100 PSI limit. 

### Total Summary

![total summary](https://user-images.githubusercontent.com/96403349/163448033-4b510b37-04fb-41cd-9d43-6c6be1ae8b68.png)

### Lot Summary

![lot-summary](https://user-images.githubusercontent.com/96403349/163448518-e9df811f-062e-47b8-94b8-f410e7df2570.png)


## T-Tests on Suspension Coils:

Perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.
The results of the t-tests OF all lots and each individual lot are below.

### Overall T-Test on Suspension coils

![2022-04-14 (7)](https://user-images.githubusercontent.com/96403349/163449562-620099d2-5c83-4f4a-a42e-a5f441cdaabf.png)

From above image we can say that the Mean of the sample is 1498.78. And the p-value is 0.06 which is higher than the significance level of 0.05, so the null hypothesis can be accepted in that there is no difference between the means of the PSI for the population and overall manufacturing lot sample. We can say that,the mean of all three of these manufacturing lots is similar to the presumed popultion mean of 1500.

### Lot1 Suspension Coil T-Test

![t test lot1](https://user-images.githubusercontent.com/96403349/163451128-f34ce2e2-426c-437e-a460-81ee93d448c0.png)

Lot1 sample has the sample mean of 1500 with the p-value is 1. That means we cannot reject or accept the null hypothesis because there is no diference between the observed sample mean and the presumed population mean of 1500.


### Lot2 Suspension Coil T-Test

![t test lot2](https://user-images.githubusercontent.com/96403349/163451838-259a2ce2-261d-4360-8bd7-d1e96959c606.png)

As lot1, lot2 has the sample mean of 1500 with the p-value is 0.06. That means the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.

### Lot3 Suspension Coil T-Test

![t test lot3](https://user-images.githubusercontent.com/96403349/163452855-d9f51901-0b2d-481c-9919-e52d71d88171.png)

Lot3 sample has the mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. And null hypothesis should be rejected in that there is a difference between the means of the PSI for the population and Lot3 and the true mean is not equal to 1500.

## Study Design: MechaCar vs Competition:

- Design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers. This study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years. To quantify how the MechaCar performs against the competition, the T-Test could be used to compare the safety ratings of MechaCar against the competition. And the next metrics should be the cost, city or highway fuel efficiency, horse power, or maintenance cost which address some safety concerns of consumers.
- The null hypothesis is that there is no difference in safety ratings between MechaCar and the competition which that means the mean of the safety rating is zero. The alternative hypothesis is that there is a difference in the safety ratings between those two groups because the mean of the safety rating is not zero.
- A multiple linear regression would be helpful to determine the statistical summary how the variables impact the safety ratings for MechaCar and their competitors.
- More random sample would need to be collected including actual variables, safety ratings, highway fuel efficiency, and horsepower and further analysis could be done by using the results from the t-test through RStudio.
