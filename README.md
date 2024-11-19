# Evaluating Demand Determinants for Yulu's Micro-Mobility Solutions

## Business Problem:

Yulu, India's pioneering micro-mobility service provider, has embarked on a mission to
revolutionize daily commutes by offering unique, sustainable transportation solutions.
However, recent revenue setbacks have prompted Yulu to seek the expertise of a consulting
company to delve into the factors influencing the demand for their shared electric cycles,
specifically in the Indian market.

## What is expected?

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

## Concepts used:

- Uni-Variate Analysis
- Bi-Variate Analysis
- 2-Sample T-test : Testing for differences across population
- ANOVA
- Chi-Square
