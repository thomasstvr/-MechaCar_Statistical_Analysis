# MechaCar Statistical Analysis


## Linear Regression to Predict MPG

Here, we have employed R to design a linear model that predicts the mpg (miles per gallon) of MechaCar prototypes based on vehicle length, weight, spoiler angle, ground clearance and whether or not the car is all wheel drive. Below is a screen shot of the script and the results:

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/Deliverable1.png)

Looking at these results, we see that vehicle length and ground clearance are statistically unlikely to cause random variance to the linear model. That is to say that vehicle length and ground clearance have a significant impact on mpg. These conclusions are drawn by focusing on the low p-value (Pr(>|t|)) of these two variables.

The slope of this model is not zero, meaning the model is of significance. We can see this by looking at the �Estimate� column in the coefficients. While vehicle weight and spoiler angle have small coefficients, the other variables have a very significant coefficient. 

The .7149 value of �Multiple R-Squared� tells us that the model is a good predictor of mpg. This number says that the model will predict the correct mpg 71.49% of the time. 

## Summary Statistics on Suspension

In this portion of the project, we have employed R to generate summary statistics of multiple production lots to determine if the manufacturing of suspension coils is consistent across the board. Below, the total summary of all three lots is shown, and below that the summary statistics of each individual lot is shown. 

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/total_summary.png)

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/lot_summary.png)

The design specifications for the MechaCar coils allow for a variance of 100 psi. If we look at the total summary of all lots, the coils are all within spec with a variance of 62.29psi. Taking a closer look at the individual lots, we see that Lot1 and Lot2 are well within spec at .98psi and 2.73psi respectively. Lot3, on the other hand, is far outside of spec at 170.29psi.

What this means is that the coil springs produced at Lot3 may be within tolerance when it comes to mean and median psi rating, they are not within tolerance when it comes to variance. That is, to many are being produced that are not within the given specifications and the manufacturing process must be reassessed. 

## T-Tests on Suspension Coils

Next, we used R to perform T-Tests on the data both as a total and based on lots. The screen shots below show the results.

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/total_ttest.png)

The t-test for the three manufacturing lots as a whole shows a p-value of .06028 and a mean of 1498.78psi

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/lot1_ttest.png)

The t-test for Lot1 shows a perfect p-value of 1 as well as a mean of 1500psi.

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/lot2_ttest.png)

Lot2�s t-test returned a p-value result of .6072 and a mean of 1500.2psi.

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/lot3_ttest.png)

Again, Lot3 falls below the significance level (.05) with a p-value of .04168. The t-test returned a mean of 1496.14psi.


## Study Design: MechaCar vs Competition

To compare the MechaCar against its competition we should first start by comparing it to all other vehicles, then move to comparing it to vehicles of the same type. Metrics of interest would be fuel economy (both city and highway), warranty (length and type of coverage), horsepower rating, 0-60 (mph) times, quarter miles times etc.

Let�s say we are targeting budget minded sports car customers who want to buy the fastest vehicle that maintains decent fuel mileage while spending less. We want to test the hypothesis that MechaCar is faster, costs less and gets better fuel mileage than the competition.  

To do this, we first collect all data of interest (price, fuel mileage, 0-60 and quarter mile times) from all available vehicles. This data would then be used to calculate the mean and standard deviation of the population then compared to that of MechaCar�s specifications. Once this has been done, we can then compare MechaCar to only other sports cars in the same manner. The more standard deviations above the competition, in fuel mileage as well as performance times, the better and vice versa for price. This then can be used to accept or reject our initial hypothesis.
