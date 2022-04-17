# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![MPG_COEF](/Images/MPG_COEF.PNG)
![LinearSummary](/Images/Linear_summary.PNG)

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

  > Vehicle length and ground clearance are statistically likely to provide non-random amounts of variance to the model. This is evidenced by the very low p value in the summary table
  
Is the slope of the linear model considered to be zero? Why or why not?


  > Firstly the multiple factor regression shows non-zero coefficients for each of the 6 factors
  > Secondly the p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. Therefire we can reject the null hypothesis, and conclude that the slope of this linear model is not zero.
 
Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

  > Yes. This linear model has an r-squared value of 0.7149, i.e. approximately 71% of all mpg values can be predictedby this model.

## Summary Statistics on Suspension Coils

The suspension coil’s PSI continuous variable across all manufacturing lots:
![Total_Summary](/Images/Total_Summary.PNG)

The suspension coil’s PSI continuous variable for each manufacturing lot:
![Lot_Summary](/Images/Lot_Summary.PNG)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

  > When looking across all manufacturing lots, PI variance 62.29 is well within the 100 PPI requirement. Similary Lot 1 (0.97) and Lot 2 (7.46) are within the 100 PPI requirement. Lot 3 (170.28) is well above the 100 PPI requirement however.

## T-Tests on Suspension Coils
All Lots:
![T_all](/Images/T_all.PNG)

Lot 1:
![T_Lot1](/Images/T_Lot1.PNG)

Lot 2:
![T_Lot2](/Images/T_Lot2.PNG)

Lot 3:
![T_Lot3](/Images/T_Lot3.PNG)

The  mean of the sample for all lots is 1498.78. With a p-Value of 0.06, there is NOT enough evidence to reject the null hypothesis. 

Looking at the individual lots: Lot 1 has a mean of 15000 and p-value of 1, Lot 2 has a mean value of 1500.2 and p-value of 0.6072. For both these lots there is no statistical difference between the observed sample mean and the presumed population mean and the high P-values mean that we cannot reject the null hypothesis.

Lot 3 on the other hand has a mean value of 1496.14 and a P-value of 0.04168. With the P-value being lower than 0.05 significance level, we can reject the null hypothsis and connclude that there IS a statistical difference between the observed sample mean and the presumed population mean.


## Study Design: MechaCar vs Competition

What metric or metrics are you going to test?

  We should look at the below metrics
  
  > Current price
  > Resale value
  > Average maintenance cost
  > Fuel efficiency MPG
  > Enging HP
  > Comfort rating
  > Safety rating
  > Brand value rating

What is the null hypothesis or alternative hypothesis?

  > Null hypothesis: MechaCar is priced right based on the above factors
  > Alternative hypothesis: MecharCar is not priced right according to the above factors
 
What statistical test would you use to test the hypothesis? And why?

  > We will perform a multiple linear regression on the above factors to determine which have the highest correlation with the price. 
  > We can also group cars by price range and do a Chisquared test on the rest of the metrics and see if there's statistical difference in any of them  
  
What data is needed to run the statistical test?

  > For each car manufacturer we will need 3 years of data for each of the metrics mentioned above

