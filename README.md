# MechaCar_Statistical_Analysis

## Part 1: Linear Regression to Predict MPG
### Deliverable 1
This analysis is to identifiy ideal vehicle performance. Multiple metrics such as vehicle length, weight, spoiler angle, drivetrain, and ground clearance, collected for each vehicle. using knowledge of R desgined a linear regress to predict mpg of MechaCar prototypes using several variables from csv file. 

Linear Regression:

<img width="778" alt="Screenshot 2023-01-06 at 21 11 47" src="https://user-images.githubusercontent.com/112133209/211132291-df540dc3-b023-42c7-b3a8-37c89d1b59ea.png">

  1. Which variables/coefficients provided a non-random amount of variancee to the mpg values in the dataset?
  
  Statistical significance on vehicle length, weight, ground clearnracne and also weight has some significant
  
  <img width="517" alt="Screenshot 2023-01-06 at 17 15 00" src="https://user-images.githubusercontent.com/112133209/211124906-9c17f816-3c9b-441f-8fd7-eca927f54153.png">
  
  2. Is the slope of the linear model considered to be zero? Why or why not?
  
  The slope of the linear model has p-value(5.35e-11) for some reason its not zero. So consdiering that signifance level islower than 0.05

  3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  
  yes R-square is neared to 1(0.175) showing variables prediction based on Vehicle length, vehicle weight, ground clearance and the rest of the variables can predict ovr 71% percent of MPG Performacnce for MechaCar Prototypes.
    
## Part 2: Create Visualiations for the Trip Analysis
### Deliverable 2
#### Summary Statistics on Suspension Coils
##### Analysis:
1. Variance for total 

The combined variance of all manufacturing batches is 62.29, which falls short of meeting the design specifications.

![Screenshot 2023-02-07 at 12 36 51](https://user-images.githubusercontent.com/112133209/217360756-4b5dbd43-8c80-4482-867a-bfe5cec3f921.png)

2. Variance for each lot

Lot-3 surpasses the design specifications with a value of 170.28, while Lot-1 (0.98) and Lot-2 (7.47) fall significantly below the design specifications.

![Screenshot 2023-02-07 at 12 37 25](https://user-images.githubusercontent.com/112133209/217361147-5beb2107-2e01-49a0-845d-8bc83518f94d.png)

In summary, the production did not meet the design specifications. The fact that Lot-3 exceeded the specifications is also a concern. Based on this preliminary analysis, it is uncertain whether the outcome is due to random chance or if the hypothesis can be rejected.
## Part 3: T-Tests on Suspension Coils
### Deliverable 3
#### Test on suspension coils
1. All manufacturing Lots vs Populations

The p-value of 0.06028 indicates a lack of sufficient evidence to reject the hypothesis

<img width="425" alt="Screenshot 2023-02-07 at 12 59 42" src="https://user-images.githubusercontent.com/112133209/217364645-21b55412-00b6-48f4-838d-5e7da6cdccf8.png">

2. Lot 1 vs Population

A p-value of 1.0 suggests that there is no evidence to reject the hypothesis, indicating that the mean of Lot-1 is equivalent to the mean of the population.

<img width="565" alt="Screenshot 2023-02-07 at 12 58 47" src="https://user-images.githubusercontent.com/112133209/217364748-2c9caf0a-91b8-4498-a766-bddb14da4048.png">

3. Lot 2 vs Population

The p-value of 0.06072 indicates a lack of sufficient evidence to disprove the hypothesis.

<img width="567" alt="Screenshot 2023-02-07 at 21 39 53" src="https://user-images.githubusercontent.com/112133209/217444567-fe8ba375-5cab-45fa-b8f4-e65277777bd6.png">

5. Lot 3 vs Population

The p-value of 0.04168 suggests that the hypothesis should be rejected, meaning the means are statistically significant.

<img width="566" alt="Screenshot 2023-02-07 at 21 40 04" src="https://user-images.githubusercontent.com/112133209/217445213-9e6bd99b-87f2-4697-88d0-c43ada7e7892.png">


### Deliverable 4
#### Study Designs: MechaCar vs Competition

The aim of the statistical analysis was to compare MechaCar to its competition. This involved the use of metric tests, formulation of null and alternative hypotheses, selection of a statistical test, and assessment of the need for the test. The hypothesis test followed a five-step process and provided an overview of the statistical results and outcomes from three lots.

The first step of the process is to test the vehicle weight and horse power using metric tests. Horse power is a measure of the car's acceleration or speed. Next, the null hypothesis (Ho: PH = 0.5) and alternative hypothesis (Ha: PH ≠ 0.5) are formulated. The results suggest the presence or absence of influences beyond chance, with a null result implying randomness. If found insufficient, further statistical analysis is necessary. The null hypothesis is evaluated using the p-value and compared with the significance level (α), which determines the importance of the findings. A significance level of 0.05 is commonly accepted, though a smaller level may be used for smaller datasets. The statistical test is then performed by computing the p-value and comparing it to the significance level. Finally, a conclusion is reached by determining whether to reject or fail to reject the null hypothesis based on the results of the tested dataset.
