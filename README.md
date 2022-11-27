
# MechaCar Statistical Analysis
Statisitical analysis of automobile performance using R.

## Overview

The purpose of this challenge is to perform an analysis to help the management of AutosRUs in understanding the production troubles that are hindering the manufacturing team's progress in their newest prototype "The MechaCar". 

Therefore, I will be performing the following analyses to help the team;

* Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.

* Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.

* Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
   
* Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers.



## Results

### Deliverable 1........................................................................................................

### Linear Regression to Predict MPG
![Multiple Linear Regression on MPG](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/mpg_linear_regres_summary.png)

* The variables that are most significant in the dataset which show a non-random effect on the MPG of the MechaCar are the **Vehicle Length** and the **Ground Clearance**. As indicated in the image above, a linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10<sup>-12</sup> and 5.21x10<sup>-8</sup>, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.
* The above image shows the p-value to be 5.35x10<sup>-11</sup>, and is lower than the extreme level of significance, and therefore, the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.
* Although there are other factors that need to be considered, however, this model predict the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149 indicates that the model is 71% accurate (i.e how well the data fit the regression model)

### Deliverable 2 .........................................................................................................
### Summary Statistics on Suspension Coils
![Suspension Coil Total Summary](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/us_coil_total_summary_1.png)
![Suspension Coil Lot Summary](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/sus_coil_total_summary_2.png)
* Although, the overall variance as shown in the total Summary data above is under 100 psi and meets specifications, however, there is a problem with one of the individual lots. The variance for Lot 3 is well above the acceptable threshold, at 170.28.


### Deliverable 3 ..........................................................................................................

### T-Tests on Suspension Coils
Suspension Coils Cumulative T-test
![Suspension Coils Cumulative T-test](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/total_sus_coil_one_sample_ttest.png)
* The review of the results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value (0.063)is higher than the level of significance (0.05) for us to reject the null hypothesis.
![Suspension Coil Lot 1 T-test](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/sus_coil_one_sample_ttest_lot1.png)
* The review of the results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) for us to reject the null hypothesis.
![Suspension Coil Lot 2 T-test](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/sus_coil_one_sample_ttest_lot2.png)
* The review of the results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis.
![Suspension Coil Lot 3 T-test](https://github.com/Adpetfem83/MechaCar_Statistical_Analysis/blob/main/Images/sus_coil_one_sample_ttest_lot3.png)
* Meanwhile, the review of the results of the T-test for the suspension coils for Lot 3 shows that they are statistically different from the population mean, and the p-value is just low enough (0.0417) for us to reject the null hypothesis. Furthermore, I think this lot needs to be discarded, or closely re-evaluated.


### Delivaerable 4 ..........................................................................................................

## Study Design: MechaCar vs Competition
Due to the fact that, there are a number of factors the customers take into consideration when evaluating a car to purchase. Thus, customers looking to buy a car are looking for more than just a conveyance. Therefore, they are looking for a car that is economically viable in terms of fuel utilization and consumption, reliable, durable, and not too expensive a car. ana,  in line with this, study can be developed to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

First and foremost, we can use a wide range of metrics to perform this analysis namely Current price, Re-sale value, MPG, Annual cost and fuel efficiency etc.
For the purpose of this study, i will use the city and highway fuel efficiency metrics.

### Null and Alternate Hypotheses
H<sub>0</sub>: MechaCar prototypes "Vehicles in the same class with the competitors have the same fuel efficiency".

H<sub>a</sub>: MechaCar prototypes "Vehicles in the same class  with the competitors do not have the same fuel efficiency".

### Statistical Test Used
The best statistical test for the purpose of this study would be multiple linear regression.

### What data is needed
The data needed for this analysis will be the information on all identified metrics over the past five years accross all the manufacturers.


