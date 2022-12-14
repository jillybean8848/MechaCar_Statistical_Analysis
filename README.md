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

Below is an image of our findings using R Studio:
![mpg](https://user-images.githubusercontent.com/110632671/205527209-89ee3a16-b3d3-41ef-b985-077a7030220c.png)

## Summary Statistics on Suspension Coils
### Total and Lot Summary
![total_summary](https://user-images.githubusercontent.com/110632671/205528033-2b966083-f8cf-42b1-8f54-f6ee53ee6b00.png)

As the image of our Total Summary Data shows above, the overall variance is under 100 PSI and meets the expected design specifications. Conversely, the Lot Summary shows an issue with one of the individual lots. Specifically, the variance in Lot 3 is over the acceptable threshold at 170.29.

### T-Tests on Suspension Coils
#### T-Test on All Lots
![All_Lots](https://user-images.githubusercontent.com/110632671/205529868-146f68ba-9885-48d4-8fd6-40f886471f8c.png)
![lot_summary](https://user-images.githubusercontent.com/110632671/205528106-9a27de42-b844-4056-81fe-c8e5fb401206.png)

This t-test was used to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds PSI. The results show that the p-value = 0.06028, which is greater than our assumed significance level at 0.05. Meaning, we do not have sufficient evidence to reject the null hypothesis. Therefore, the PSI across all manufacturing lots is statistically similar to the population mean of 1,500 pounds PSI.

### Lot 1
![Lot1](https://user-images.githubusercontent.com/110632671/205530359-0c3d42d7-f4a0-4149-b5b2-19a4c71dd638.png)

T-test for Lot 1 shows a p-value of 1 which is greater than our assumed signficance level of 0.5. Therefore, it is not statistically different from the population mean and the p-value is not low enough to reject the null hypothesis.

### Lot 2
![Lot2](https://user-images.githubusercontent.com/110632671/205530403-e7fe604a-ad8d-47ba-960d-aa104a2687fc.png)

Results of the T-test for Lot 2 shows a p-value of 0.6072, which is greater than our assumed significance level of 0.05. Therefore, it is not statistically different from the population mean, and the p-value is not low enough to reject the null hypothesis.

### Lot 3
![Lot3](https://user-images.githubusercontent.com/110632671/205530418-d6da2a29-5c3e-41fa-96b4-5d3c7720918d.png)

T-test results for Lot 3 shows a p-value of 0.04168, which is smaller than our assumed significance level of 0.05. Therefore, we do have sufficient evidence to reject the null hypothesis. 

## Study Design: MechaCar vs Competition
### 1. What metric or metrics are you going to test?
The next metrics I would be interested in testing would be safety ratings, fuel efficiency and horsepower.

### 2. What is the null hypothesis or alternative hypothesis?
Horsepower:
Null Hypothesis: The means of horsepower of all vehicles in this class are equal.

Alternative Hypothesis: At least one of the vehicles in this class has a different mean of horsepower than other vehicles.

Fuel efficiency:
Null Hypothesis: The means of fuel efficiency of all vehicles in this class are equal.

Alternative Hypothesis: At least one of the vehicles in this class has a different mean of fuel efficiency than other vehicles.

Safety rating:
Null Hypothesis: The means of safety ratings of all vehicles in this class are equal.

Alternative Hypothesis: At least one of the vehicles in this class has a different mean of safety rating than other vehicles.

### 3. What statistical test would you use to test the hypothesis? And why?
I would use statistical T-tests for this hypothesis because t-tests can compare the population of all our vehicles and competitors vehicles.

### 4. What data is needed to run the statistical test?
Data needed to run statistical testing would be testing from the MechaCar and test data for each of our competitors vehicles.









