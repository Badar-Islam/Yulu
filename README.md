# Evaluating Demand Determinants for Yulu's Micro-Mobility Solutions

## Business Problem:

Yulu, India's pioneering micro-mobility service provider, has embarked on a mission to
revolutionize daily commutes by offering unique, sustainable transportation solutions.
However, recent revenue setbacks have prompted Yulu to seek the expertise of a consulting
company to delve into the factors influencing the demand for their shared electric cycles,
specifically in the Indian market.

## Objective:

The company wants to know:
- Which variables are significant in predicting the demand for shared electric cycles in the
Indian market?
- How well those variables describe the electric cycle demands

## Column Profiling:

|Column |	Description|
|-------|------------|
|datetime |	datetime|
|season	| season (1: spring, 2: summer, 3: fall, 4: winter)|
|holiday |	whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)|
|workingday |	if day is neither weekend nor holiday is 1, otherwise is 0.|
|temp |	temperature in Celsius|
|atemp |	feeling temperature in Celsius|
|humidity |	humidity|
|windspeed |	wind speed|
|casual	| count of casual users|
|registered |	count of registered users|
|count | Total_riders	count of total rental bikes including both casual and registered|

<b>weather</b>:
|Category |	Details|
|---------|--------|
|1	| Clear, Few clouds, partly cloudy, partly cloudy|
|2	| Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist|
|3	| Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds|
|4	| Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog|

## Concepts Used:

- Uni-Variate Analysis
- Bi-Variate Analysis
- 2-Sample T-test : Testing for differences across population
- ANOVA
- Chi-Square

## Tasks Performed:

- Loaded the dataset and performed basic EDA to understand its characterstics and structure.
- Performed data Cleaning like missing value handling, checking for duplicate values, fixing Structural Errors, handling outliers etc.
- Performed non graphical analysis such as descriptive analysis, frequency distribution, cross-tabualtion, correlation analysis etc.
- Visualizations :
    - Uni-Variate Analysis (distribution plots of all the continuous variable(s) barplots/countplots of all the categorical variables)
    - Bivariate (Relationships between important variables such as workday and count, season and count, weather and count)
- For continuous variable(s): Distplot, countplot, histogram for univariate analysis
- For categorical variable(s): Boxplot
- For correlation: Heatmaps, Pairplots
- Performed approriate testing on following:
  - Working Day has effect on number of electric cycles rented
  - No. of cycles rented similar or different in different seasons
  - No. of cycles rented similar or different in different weather
  - Weather is dependent on season
- Performed Hypothesis Testing:
  - Setup Null Hypothesis (H0)
  - State the alternate hypothesis (H1)
  - 2-Sample T-Test to check if Working Day has an effect on the number of electric cycles rented
  - ANOVA to check if No. of cycles rented is similar or different in different weather and/or season
  - Chi-square test to check if Weather is dependent on the season
- Checked assumptions of the test like:
  - Normality using Histogram, Q-Q plot, skewness or Shapiro-wilk test and
  - Equality Variance using levene’s test.
- Based on observation provided business insights and recommendations.


