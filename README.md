# MechaCar_Statistical_Analysis

# Overiview

Jeremy, a 10 yr tenure employee at AutosRUs has been tasked with a role of data analyst in the Data Analytics team. The leadership team has assigned Jeremey with a new project to perform statistical tests on their datasets for a prototype vehicle called "MechaCar". The new prototype is facing some production challenges and the leadership team is hoping that the analytical team can provide some insights on the issues that need to be addressed and fixed. Jeremey along with the Data Analytics team decide on the below approach:
1. Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
2. Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
3. Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
4. Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers.

## Linear Regression to Predict MPG
<img   src=""  alt="UFO Sightings"  title="UFO Sightings" style="display: inline-block; margin: 0 auto; max-width: 300px">


## Statistical Summary:

1. The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. 
   The variable p-values of 2.6x10-12 and 5.21x10-8, respectively, indicate that they have statistically significant impact on fuel efficiency. 
   The y- intercept was also statistically significant, indicating that there are likely other factors that have a strong impact on the MPG but were not included in        our dataset.   
2. The models p-value of 5.35x10-11, is significantly lower than the assumed significance level of 0.05% and thus the slope of the linear model cannot be considered to      be zero. This also supports their statistical decision to reject the null hypothesis of slope being zero.
3. The coefficient of determination (r-squared) value of 0.7149 indicates that this linear model does indeed predict mpg of MechaCar prototypes fairly well, although        there are many unconsidered factors.
