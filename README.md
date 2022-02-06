# MechaCar_Statistical_Analysis

##Overview

AutosRUs’ new prototype the MechaCar is suffering from production troubles that are blocking the manufacturing team’s progress. By helping Jeremy compare the datasets from the two CSV files, we will be able to identify hiccups in the manufacturing process and provide upper management the details on areas that need to be addressed. 
By using R Studio and various statistical analysis, the manufacturing issues analysis will be easily displayed and explained to upper management in a comprehensive and clear manner.

Linear Regression to Predict MPG:

The summary ouput from the linear regression function provided key insight into which factors influenced the car's MPG rating. Main findings include:
The vehicle's length (at a p-value of 2.6 * 10^-12) and the vehicle's ground clearance (at a p-value of 5.21 * 10^-8) were two variables that provided non-random amounts of variance to the MPG values based on this dataset.
The slope of the linear model is not considered to be zero because the returned p-value of 5.35 * 10^-11 is below the necessary p-value threshold of 0.05. This shows evidence to reject a null hypothesis, and that the linear model has a slope that can predict the data points with a high degree of accuracy.
The linear model predicts the MPG rating of MechaCar prototypes effectively due to the R-squared value of 0.715, indicating a positive correlation coefficient. With the R-squared value showing a closer value to 1.0 than 0.5 it predicts the MPG values with a higher degree. With this R-squared value combined with the p-value supporting a greater probability of accuracy than random chance, this linear model can be deemed effective in predicting the MPG values. The linear model is effective in predicting some known data values available, but its accuracy in predicting future values that are not presently available should not be deemed 100% reliable. 

Summary Stats on Suspension Coils:

The variance in the pressure levels recorded for the coils does not satisfy the required specifications in the design specifications for MechaCar's suspension coil manufacturing in all cases. The variance is deemed to be within an acceptable range for the values if the the coils produced from all manufacturing lots is considered an absolute.

When taken individually, Lot3’s variance in suspension coil pressure ratings exceeded the specified limit by a difference of over 70 PSI. Also indicated by the Standard Deviation value the quality of the coils produced at Lot3 are not up to par in consistency with the other sites.  

T-Tests on Suspension Coils:

By running a T-test for the product records of all the manufacturing lots and then running a test individually for each lot showed many differences in the mean values field compared to the given population mean of 1500. It also shows the deviations from the population mean which lot had a greater variation than the other lots.  

Overall Test:

The T-test for all suspension coil records against the population mean is presented in the screenshot t_tests_all.png

The initial T-test showed a t value of -1.89, and a p-value of 0.06. The variation is not particularly noteworthy and by working with the common threshold for p-values to be below 0.05 for rejection of the null hypothesis, the difference between the mean values is not high enough to consider them statistically impactful.  

Individual Lot Tests:

In order to understand the mean coil PSI values by lot, the t-values and p-values provide context for why the values were off in the overall test but not by any significant margin. See t_tests_lots.png 

Lot 1 values have a steady connection to the population mean value due to the t-value listed at zero and the p-value listed at one. 

Lot 2 values show a minor variation with the t-value less than 1.0 and the p-value higher than 0.05 which are not deemed to be statistically impactful.  

Lot 3 values show a t-value of -2.1 and a p-value of 0.042. The -2.1 t-value surpassed the overall t-value result and taken with the p-value make the value quite skewed / statistically impactful, but still confirms the rejection of the null hypothesis. Due to Lot 3 values being so skewed this shows that the analysis of Lot 3’s mean PSI value was an impactful factor when reviewing the results for the group of lots. 

Conclusion - MechaCar vs Competition:

In order to compare the MechaCar prototype versus outside competition an analysis on similar manufacturing factors would need to be conducted. A proposed comparison would be to investigate two specific performance criteria of the MechaCar prototype and its competitors to see who would come out on top. Please see the details of the analysis below: 

Consumers will most likely want to compare the city and highway MPG efficiency and the total cost of the vehicle.

The null hypothesis / alternative hypothesis would be consistent fuel efficiency across city/highway and the average car prices being consistent with the total size and class of the vehicle. 

The statistical test for these metrics would be:

1. A linear regression test would compare the speed and fuel level after completing test drives over the same stretch of distance.
2. Comparing the total manufacturing and materials costs for the MechaCar prototype versus its competitors would require two-sample T-tests to get a full analysis. 

The data would need to consist of dependent and independent variables such as MPG values calculated over driven stretches of roads and then see how much fuel is left in the tank at each point after the road tests. Then you would need to calculate the cost of the materials needed to manufacture the vehicles and then compare to similar model competitors in the sedan class, SUV, mid-size, compact etc.  

 