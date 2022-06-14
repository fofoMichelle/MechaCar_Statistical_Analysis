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
- 
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




