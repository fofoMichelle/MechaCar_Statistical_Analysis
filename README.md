# MechaCar_Statistical_Analysis
# Overview and Purpose

The purpose of this analysis is to create an analysis on the AutosRUs's newest prototype "MechaCar" which is suffering from production troubles that are blocking the manufacturing team's progress.
They put Jeremy our contact within the company, on a special project to review the production data for insights that may help the manufacturing team.

The following tasks will be performed to complete the project:
- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Resources

### Data
- MechaCar_mpg.csv Suspension_Coil.csv

### Software

- R 4.2.0
- RStudio

## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/99924850/173481915-4a0407fc-eca3-4d06-b6f4-e8e6faf0acfc.png)


- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

According to our results, ( if we take a look at our (Pr(>|t|) values) vehicle length and ground clearance (as well as intercept) are statistically unlikely to provide random amounts of variance to the linear model. In other words the vehicle length and ground clearance have a significant impact on mpg.

- Is the slope of the linear model considered to be zero?

We would run the following hypothesis to answer this question:
H0 : The slope of the linear model is zero

Ha: The slope of the linear model is not zero

 assumed significance level is 0.05 

Our p-value =5.35e-11

p-value<0.05

We can then reject the null hpothesis which means that the slope of the linear model is not zero.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

R-squared of approximately 0.7149. This indicates that the multiple linear regression will predict 71% of mpg observations.

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

According to this image the variance of the suspension coils  in total is 62.29356 which is less than 100 therefore the current manufacturing data meet this design specification for all manufacturing lits in total 


![image](https://user-images.githubusercontent.com/99924850/173484213-968544bc-faa4-43ec-a129-09e493e05513.png)

Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually?



![image](https://user-images.githubusercontent.com/99924850/173484647-8ab852d6-0ca1-46cc-9cf8-a398969616d3.png)

Individually we can see that Lot 1 and Lot 2 do meet the requirements however Lot 3 does not meet the requirement as its variance is approximatevely 170.3

## T-Tests on Suspension Coils

Below are the T-test results . We will assume the significance level of 0.05 percent and look at our p value:

### All manufacturing lots 

At an assumed significance level of 0.05 percent, our p-value of 0.06 is above the significance level. Therefore, we do not have sufficient evidence to reject that there is a statistical difference between All Manufactuting lots and the population mean. The two means are statistically similar.

![image](https://user-images.githubusercontent.com/99924850/173485612-35b57276-0af0-425c-8364-95a9fe9d810b.png)

### Lot 1 

![image](https://user-images.githubusercontent.com/99924850/173486654-a845fc93-87fc-4b32-a5d5-d1663059bb3f.png)

At an assumed significance level of 0.05 percent, our p-value of 1.0 is above the significance level. Therefore, we do not have sufficient evidence to reject that there is a statistical difference between Lot 1 and the population mean. The two means are statistically similar.

### Lot 2

![image](https://user-images.githubusercontent.com/99924850/173486786-a85568ed-9889-48af-8c7c-2ffed53b425d.png)

At an assumed significance level of 0.05 percent, our p-value of 0.61 is above the significance level. Therefore, we do not have sufficient evidence to reject that there is a statistical difference between Lot 2 and the population mean. The two means are statistically similar.

### Lot 3

![image](https://user-images.githubusercontent.com/99924850/173486915-9d62bbfe-4e3b-4c00-a601-b9c2b99c816b.png)

At an assumed significance level of 0.05 percent, our p-value of 0.042 is below the significance level. There is sufficient statistical evidence to reject that there is a statistical difference between Lot 3 and the population mean. The two means are statistically different.

## Study Design: MechaCar vs Competition

To compare MechaCar to its competition one can use an ANOVA test to compare the MechaCar in alot of categories that would matter to customers including but not limited to  cost, city or highway fuel efficiency and maintenace cost.
With the ANOVA test we will be able to test if the means from multiple sampleas are significantly similar or different.
We would gather data from the competition cars and compare the average of these cars in different categories to the ones from MechaCar.
The p value being greater than 0.005 would mean that the MechaCars has the same performances within these categories would be our null hypothesis.And the opposite would be the alternative hypothesis.
If the p value is less than 0.05  we are to reject our null hypothesis. We would then need to look at the average of the MechaCar if either below or above the other average this would show its performance against its competitors with below being worse and above being better.












