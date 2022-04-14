# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG 

![Summary 1](https://user-images.githubusercontent.com/96403349/163402180-632abcf5-40bb-4b55-8421-409f4042edbd.png)

1) The above screenshot we can see the the results of producing a linear regression model to predict MPG from the MechaCar_mpg dataset by using the variables of vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD. So the vehicle length, and ground clearance are statistically likely to provide non-random amounts of variance to the model which significant impact on miles per gallon on the MechaCar prototype. However, the vehicle weight, spoiler angle, and AWD ( All Wheel Drive) have p-Values that indicate a random amount of variance with the dataset.

2)  The slope of the linear model is not considered to be zero because the estimates for all coefficients are not zero. This is because, p-value is 5.35e-11 which much smaller than the significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, and slope of this linear model is non zero. 

3) This linear model predicts the mpg of MechaCar protoypes effectively because the Adjusted R-squared reflects that 0.7149, which means that approximately 71% of the variation within mpg is explained by the coefficients.

