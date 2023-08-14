# BIKE_SHARING_ASSIGNMENT
> To find the variables affecting the demand for the shared bikes to make more profit.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

the factors affecting the demand for these shared bikes in the American market. The company wants to know:
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

We are using Bike share dataset

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- Numpy -- version -1.24.3
- Pandas -- version -1.4.2
- Matplotlib -- version -3.5.1
- Seaborn -- version -0.11.2
- Scikit Learn -- version -1.0.2
- Statsmodels -- version -0.13.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Conclusions
- No missing values in the Dataset
- Visualizing the data in lineplot between variables 'Year-Month' and 'cnt' Bookings have dropped significantly because of spring time and christmas days.
- Visualizing the pairplot btween the variables 'temp','atemp', 'hum', 'windspeed', 'cnt' we can clearly see the 'temp' is significant variable for Model
- Bar plot visualization for correlation.
  1. seasons - Spring is negatively highly correlated and where as summer,fall and winter as posiively correlated 
  2. months - nov,dec,jan,feb,march negatively correlated and where others are positively
  3. weekdays - there is no much of correlation explained in weekdays
  4. weather - clear weather is positively correlated and haze and percipitation are negatively
  5. yr - year is high correlated with cnt
  6. temp & a_temp - are also highly correlated with cnt

- We can see that the equation of our best fitted line is:

$cnt$ = 0.1959 - 0.1086 X $spring$ + 0.0350 X $summer$ + 0.0833 X $winter$ + 0.0438 X $mar$ - 0.0561 X $jul$ + 0.0572 X $sep$ - 0.0389 X $dec$ - 0.0418 X $tue$ - 0.0841 X $haze$ - 0.2737 X $precipitation$ + 0.02529 X $yr$ + 0.4884 X $temp$ - 0.1004 X $windspeed$

## Acknowledgements
- This project was given by UpGrad
