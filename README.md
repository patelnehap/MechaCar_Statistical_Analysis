# MechaCar_Statistical_Analysis

# Overiview

Jeremy, a 10 yr tenure employee at AutosRUs has been tasked with a role of data analyst in the Data Analytics team. The leadership team has assigned Jeremey with a new project to perform statistical tests on their datasets for a prototype vehicle called "MechaCar". The new prototype is facing some production challenges and the leadership team is hoping that the analytical team can provide some insights on the issues that need to be addressed and fixed. Jeremey along with the Data Analytics team decide on the below approach:
1. Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
2. Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
3. Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
4. Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers.

## Linear Regression to Predict MPG

## Statistical Summary:

<img   src="https://github.com/patelnehap/MechaCar_Statistical_Analysis/blob/main/Images/Linear_Regression_1.JPG"  alt="LM Analysis"  title="LM Analysis" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. 
   The variable p-values of 2.6x10-12 and 5.21x10-8, respectively, indicate that they have statistically significant impact on fuel efficiency. 
   The y- intercept was also statistically significant, indicating that there are likely other factors that have a strong impact on the MPG but were not included in        our dataset.   

<img   src="https://github.com/patelnehap/MechaCar_Statistical_Analysis/blob/main/Images/Linear_Regression_2.JPG"  alt="LM Analysis"  title="LM Analysis" style="display: inline-block; margin: 0 auto; max-width: 300px">

2. The models p-value of 5.35x10-11, is significantly lower than the assumed significance level of 0.05% and thus the slope of the linear model cannot be considered to      be zero. This also supports their statistical decision to reject the null hypothesis of slope being zero.
3. The coefficient of determination (r-squared) value of 0.7149 indicates that this linear model does indeed predict mpg of MechaCar prototypes fairly well, although        there are many unconsidered factors.

## Summary Statistics on Suspension Coils
<img   src="https://github.com/patelnehap/MechaCar_Statistical_Analysis/blob/main/Images/Total_Summary.JPG"  alt="Total Summary"  title="Total Summary" style="display: inline-block; margin: 0 auto; max-width: 300px">

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
Total Summary statistics, as per the above image, indicates that the current manufacturing data meets the requirement for the toal lot. 

<img   src="https://github.com/patelnehap/MechaCar_Statistical_Analysis/blob/main/Images/Lot_Summary.JPG"  alt="Lot Summary"  title="Lot Summary" style="display: inline-block; margin: 0 auto; max-width: 300px">

But when the detailed lot summary is reviewed,as per the above image, lot 3 exhibits the issue. The variance for Lot 3 is well over the acceptable threshold (100 PSI), at 170.28.
So while the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with one of the individual lots (Lot 3).

## T-Tests on Suspension Coils

<img   src="https://github.com/patelnehap/MechaCar_Statistical_Analysis/blob/main/Images/T_Test_All.JPG"  alt="T- Tests"  title="T-Tests" style="display: inline-block; margin: 0 auto; max-width: 300px">


As per the image above,the results of the T-test for the suspension coils across all manufacturing lots were analyzed. The analysis indicates that they are not statistically different from the population mean (1498.78), and the p-value (0.06028) is not low enough for us to reject the null hypothesis.

<img   src="https://github.com/patelnehap/MechaCar_Statistical_Analysis/blob/main/Images/T_Test.JPG"  alt="T Tests by Lot"  title="T Tests by Lot" style="display: inline-block; margin: 0 auto; max-width: 300px">

A review of the results of the T-test for the suspension coils for Lot 1 and Lot 2 indicate that they are not statistically different from the population mean (1500,1500.2 respectively), and the p-value (1, 0.6072 respectively) is not low enough  for us to reject the null hypothesis.
However, Lot 3 results indicate that they are slightly statistically different from the population mean (1496.14), and the p-value (0.04168) is just low enough  for us to reject the null hypothesis. This lot may be need to be closely evaluated for improvements.

## Study Design: MechaCar vs Competition

AutosRUs is working round the clock to improve their new Mechacar prototype. The company also needs to analyze their competitors car feature to get some market share and recognition within their customer base. The main features that need to be assessed are cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating. 

## Metric to test

Although there a multitude of possible metrics to consider,  Jeremy would like to assess and compare the cars gasoline efficiency. 

## Null and Alternate Hypothesis

Null Hypotheses:Mechacar's gasoline efficinecy is statistically same or better than the competitor's avg MPG in the same automobile  category.
Alternate Hypotheseis: There is statstical difference in gasoline efficiency between Mechacar and its competitors.

## Statistical Test 

Since the feature that Jeremy wants to analyze is categorical and an independant variable it would be best for him to run the ANOVA statistical test.
Jeremy would need to collect data from various competitors and Mechacar prototype to run a statistical test. The data required would be how much MPG does the vehicles from different competitors give compare it to Mechacar, run the null/alternate hypothesis to analyze the results.



