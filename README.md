# MechaCar Statistical Analysis


## Linear Regression to Predict MPG
Here, we have employed R to design a linear model that predicts the mpg (miles per gallon) of MechaCar prototypes based on vehicle length, weight, spoiler angle, ground clearance and whether or not the car is all wheel drive. Below is a screen shot of the script and the results:

![]( https://github.com/thomasstvr/MechaCar_Statistical_Analysis/tree/main/Resources)

Looking at these results, we see that vehicle length and ground clearance are statistically unlikely to cause random variance to the linear model. That is to say that vehicle length and ground clearance have a significant impact on mpg. These conclusions are drawn by focusing on the low p-value (Pr(>|t|)) of these two variables.

The slope of this model is not zero, meaning the model is of significance. We can see this by looking at the ‘Estimate’ column in the coefficients. While vehicle weight and spoiler angle have small coefficients, the other variables have a very significant coefficient. 

The .7149 value of ‘Multiple R-Squared’ tells us that the model is a good predictor of mpg. This number says that the model will predict the correct mpg 71.49% of the time. 


