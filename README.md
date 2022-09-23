# MechaCar Statistical Analysis
## Overview
### Purpose
The company MechaCar is wanting to review their production mechanisms to increase efficiency. The goal of the project is to uncover which variables predict the MPG for vehicle prototypes, collect summary statistics on the PSI of suspension coils, determine if manufacturing lots are statistically different from the mean population, and to design a study that compares the MechaCar performance against vehicles from other manufacturers. 
## Results
### Linear Regression to Predict MPG
![linear ss](https://user-images.githubusercontent.com/106560739/191884262-35245f43-18dc-4c26-8645-5e70cdbf8944.png)
* The most significant variables in the dataset that show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. Running a linear regression model for these variables against figures for MPG resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors that have a strong impact on the MPG. 
* The slope of the linear model cannot be zero, as the p-value of 5.35x10-11 is lower than even an extreme level of significance. This means that the null hypothesis must be rejected. Therefore, the relationship between the variables and the miles per gallon is subject to more than random chance.
* Although there are still unconsidered factors, this model does predict the MPG of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149 indicates that the model is 71% accurate.
### Summary Statistics on Suspension Coils
![total_summary](https://user-images.githubusercontent.com/106560739/191885056-3400427b-775b-4078-bf6b-cd41af02a45a.png)
![lot_summary](https://user-images.githubusercontent.com/106560739/191885073-99b807f9-90a1-4d7a-8571-f46bccf133c0.png)
* While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with one of the individual lots. As shown in the Lot Summary stats, the variance for Lot 3 is above the acceptable threshold, with a value of 170.28.
### T-Tests on Suspension Coils
![one sample t-test 1](https://user-images.githubusercontent.com/106560739/191885298-1ffd9d4e-0dbc-4a77-a4d9-c0ca9fc68f87.png)
* The T-test for the suspension coils across all manufacturing lots shows that lots are not statistically different from the population mean. Also, the p-value is not small enough (0.0603) to reject the null hypothesis.
![lot 1 sample t-test](https://user-images.githubusercontent.com/106560739/191885466-44ec9403-7e6c-47ec-af2e-55d5dd9a7cec.png)
* The T-test for the suspension coils for Lot 1 shows that it is not statistically different from the population mean. The p-value is not low enough (1) to reject the null hypothesis. 
![lot 2 sample t-test](https://user-images.githubusercontent.com/106560739/191885547-b8334b7e-3a70-4919-ab6e-b07653cec6d6.png)
* The T-test for the suspension coils for Lot 2 shows that it is not statistically different from the population mean. The p-value is small enough (0.6072) to reject the null hypothesis.
![lot 3 sample t-test](https://user-images.githubusercontent.com/106560739/191885620-6b61fb6f-25a8-4e38-9b07-42a6b7de7dcd.png)
* 

