# MechaCar_Statistical_Analysis
## Overview
AutosRUs' newest prototype, MechaCar, is suffering from production troubles that are blocking manufacturing process. The company is hoping that an analytical review may help provide some insight. The goal of this project is to:
 
  * Perform multiple linear regression analysis' to identify which variables in the dataset predict the mpg of MechaCar prototypes
  * Collect summary statistics on the (PSI) of the suspension coils from the manufacturing lots
  * Run t-tests to determine if the manufacturing lots are statistically different from the mean population
  * Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 
  
 ## Results
 
 ## Linear Regression to Predict MPG
  The MechaCar dataset contains a sample size of 50 prototypes measuring the miles per gallon across multiple variables. The linear regression was calculated using R in RStudio.

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  * Vehicle length and ground clearance provided non-random amounts of variance. To note, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance within the dataset.

2. Is the slope of the linear model considered to be zero? Why or why not?
  * The p-Value for this model showed to be: 5.35e-11, which is lower than an extreme level of significance. This indicates that there is enough evidence to reject our null hypothesis. 

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  * Although there are still many alternative factors that have not been considered this model does predict the mpg of the MechaCar prototype with some level of effectiveness. The r-squared value of 0.7149 indicates that the model is 71% accurate. Meaning it can help to make predictions although an alternative method may perform with a higher level of accuracy. 
