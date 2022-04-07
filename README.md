## Linear Regression to Predict MPG
- The variables that provided a non-random amount of variance to the MPG of the values were the Intercept, Vehicle Length, Ground Clearance and maybe Weight since it was close to the 5% cutoff (7%). Overall, this data shows evidence of overfitting and cannot accuratly predict future data. 
- The slope is not considered to be 0 since there are factors that have significant impact to MPG, shown by their P values. 
- This linear model does not predict the MPG of the prototypes effectively since the intercept is showing signs of overfitting and therefore cannot accurately predict future values. 

## Summary Statistics on Suspension Coils
- While the total PSI variance across all lots is less than the threshhold(top image), Lot 3 does not meet the individual standards. Shown below, the vairance of Lot 3 individually is ~170 PSI - well over the 100 PSI threshhold, (bottom image). 

![Summary Statistics](https://github.com/dylanvowell/MechaCar_Statistical_Analysis/blob/main/summary_stats.png?raw=true) 

![Lot Statistics](https://github.com/dylanvowell/MechaCar_Statistical_Analysis/blob/main/Lot_Summaries.png?raw=true)

## T-Tests on Suspension Coils
- According to the t-test results, the mean of PSI across all lots compared to the observed mean has a p-value of .06028 - which means we reject the null hypothesis that there is no difference. See test results below: 

![Test Results](https://github.com/dylanvowell/MechaCar_Statistical_Analysis/blob/main/t_test%20summaries.png?raw=true)

- Out of the individual lots, only Lot3 was different enough from the observed mean to reject the null hypothesis. 

- Since the mean of all samples was very close to the .05 cutoff, more samples would need to be taken from the population in order to determine if there really is a significan statistical difference between what the observed mean was vs. samples. 

## Study Design: MechaCar vs Competition

An effective study comparing MechaCar to their competition would first start with determining what consumers look for in a car. According to the [NY Times
](https://www.nydailynews.com/autos/buyers-guide/10-top-reasons-people-buy-specific-cars-article-1.2552707), the top 10 things consumers consider when purchasing a car are: Reliablilty, Style, Previous Experience with the Brand, Reputation/Reviews, Performance, Price, Safety/Fuel Economy, Quality of Workmanship, and whether or not the car is 2 or 4 wheel drive. Bearing that in mind, we would need to identify the factors which are relevant across all consumer needs and easily quantifiable. This means we only have use for Reliability, Performance, Price, Safety Rating, Fuel Economy, and Style (depending on the demographic we are going after). 

Our Null Hypothesis would be that there is no difference between average performance of MechaCar vs. Competitors. We would use the above metrics in our study, but would need to potentially include Style and drivetrain (4 wheel drive vs 2 wheel) if we were going to dig deeper into different car types, i.e minivans, pickup trucks, sports cars, etc. These would be more appealing depending on the demographic you're a part of, so it's important to not only show the overall summary, but also the summaries of each type. I believe using a two sided T-Test would be best for this since you are going to be comparing a sample of MechaCar data and a sample of the competition's data. You would do this test for overall performance, as well as for each category individually to determine if MechaCar is up to par with everyone else. 
