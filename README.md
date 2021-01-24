# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

    The variables that provided a non-random amount of variance to the mpg value were vehicle_length & ground clearance, due to their small sizes of 2.660e-12 & 5.21e-08 respectively.

2. Is the slope of the linear model considered to be zero? Why or why not?

    The slope of our linear model is not considered to be zero because the p-value of 5.35e-11 is smaller that the significance level of 0.05%

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

    Yes, with the Multiple-R Squared value of 0.7149 it is an effective tool to predict mpg of MechaCar Prototypes.

## Summary Statistics on Suspension Coils

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

    The current manufacturing data meets the design specification for all the lots together but not for each lot individually, the total variance for all the lots together is 62.29356, which passes, while lot 3s variance is 170.2861224 which does not meet the specification of having a variance not exceeding 100psi.
![total_summary](https://github.com/ccastanette/MechaCar_Statistical_Analysis/blob/main/pics/total_summary.png)

![per_lot](https://github.com/ccastanette/MechaCar_Statistical_Analysis/blob/main/pics/lot_summary.png)
## T-Tests on Suspension Coils

The results of the t.test for the whole population of the suspension_Coil data is a p-value of .06028 which means that the mean of the population is not statistically different from 1500.
![total_pop_ttest](https://github.com/ccastanette/MechaCar_Statistical_Analysis/blob/main/pics/pop_t_test.png)

For each of the lots the p-values are:
Lot 1: 1

![lot1](https://github.com/ccastanette/MechaCar_Statistical_Analysis/blob/main/pics/lot1_t_test.png)

Lot 2: .6072

![lot2](https://github.com/ccastanette/MechaCar_Statistical_Analysis/blob/main/pics/lot2_t_test.png)

Lot 3: .04168

![lot3](https://github.com/ccastanette/MechaCar_Statistical_Analysis/blob/main/pics/lot3_t_test.png)

This means that of the 3 lots only Lot 3 has a mean that is statistically different than 1500.

## Study Design: MechaCar vs Competition

1. What metric or metrics are you going to test?
    
    I am going to test city and highway mileage of the mechaCar vs the 3 most popular competitor cars of the same class.

2. What is the null hypothesis or alternative hypothesis?
    
    The null hypothesis is that the city and highway mileage the mechacar gets is not related to either of the competitors. The alternative hypothesis is that they will be significantly related.

3. What statistical test would you use to test the hypothesis? And why?

    I would use the two-sample t-test using samples from the mechacar data as well as samples from the three main competitors data to see if the mean of the samples is statistically different. If not then the alternative hypothesis holds up and we are on the right track in giving our mechacar a fuel economy that will be popular.

4. What data is needed to run the statistical test?

    We will need to collect mpg data for both city and highway from each of our 3 main competitors.


