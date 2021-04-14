# MechaCar Statistical Analysis


## Linear Regression to Predict MPG

Here, we have employed R to design a linear model that predicts the mpg (miles per gallon) of MechaCar prototypes based on vehicle length, weight, spoiler angle, ground clearance and whether or not the car is all wheel drive. Below is a screen shot of the script and the results:

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/Deliverable1.png)

Looking at these results, we see that vehicle length and ground clearance are statistically unlikely to cause random variance to the linear model. That is to say that vehicle length and ground clearance have a significant impact on mpg. These conclusions are drawn by focusing on the low p-value (Pr(>|t|)) of these two variables.

The slope of this model is not zero, meaning the model is of significance. We can see this by looking at the ‘Estimate’ column in the coefficients. While vehicle weight and spoiler angle have small coefficients, the other variables have a very significant coefficient. 

The .7149 value of ‘Multiple R-Squared’ tells us that the model is a good predictor of mpg. This number says that the model will predict the correct mpg 71.49% of the time. 

## Summary Statistics on Suspension

In this portion of the project, we have employed R to generate summary statistics of multiple production lots to determine if the manufacturing of suspension coils is consistent across the board. Below, the total summary of all three lots is shown, and below that the summary statistics of each individual lot is shown. 

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/total_summary.png)

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/blob/main/Resources/lot_summary.png)

The design specifications for the MechaCar coils allow for a variance of 100 psi. If we look at the total summary of all lots, the coils are all within spec with a variance of 62.29psi. Taking a closer look at the individual lots, we see that Lot1 and Lot2 are well within spec at .98psi and 2.73psi respectively. Lot3, on the other hand, is far outside of spec at 170.29psi.

What this means is that the coil springs produced at Lot3 may be within tolerance when it comes to mean and median psi rating, they are not within tolerance when it comes to variance. That is, to many are being produced that are not within the given specifications and the manufacturing process must be reassessed. 

## T-Tests on Suspension Coils




## Study Design: MechaCar vs Competition


