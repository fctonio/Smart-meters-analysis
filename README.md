<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Statistical-Analysis-Project
*Paul Musco, Mayowa Akinyele and Anton Neike*

*Data-ber-08-20, Berlin & 16/09/2020*

## Content
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Repository organisation](#repository-organisation)
- [Results/findings](#results-findings)
- [Potential improvements/future analysis](#potential-improvements-future-analysis)

## Project Description

The goal of this project is to create and interprete different types of visualizations using real world data as well as statistical analysis. For this project we worked in a group of three people and had to choose our own subject and data. The goal is to hold a presentation of 5 minutes at the end of the week and present our finding in a way anyone could understand.

## Dataset

For this project, we used a dataset sourced from Kaggle looking at energy consumption in London, weather conditions over the same period and Acorn groups. We downloaded the following datasets from Kaggle:<br>
<br>
- acorn_details.csv<br>
- daily_dataset.csv<br>
- informations_households.csv<br>
- uk_bank_holidays.csv<br>
- weather_daily_darksky.csv<br>
<br>
The original datasets can be downloaded from the following link: https://www.kaggle.com/jeanmidev/smart-meters-in-london<br>
<br>
We used statistical analysis skills to analyze these datasets, the resulting CSV files are:<br>
<br>
- acorn_demog (daily_dataset.csv & informations_households.csv merged, ACORN groups as index)<br>
- daily_dataset_clean (cleaned version of Kaggle original)<br>
- daily_group_households_merge (daily_dataset.csv (grouped by ‘LCLid’) & informations_households.csv merged)<br>
- daily_weather_merge ('weather_daily_darksky_clean.csv' & 'daily_dataset_clean.csv' merged, needed for regression)<br>
- households_accom_merge (daily_dataset.csv & informations_households.csv merged, categories as index)<br>
- weather_daily_darksky_clean (cleaned version of Kaggle original)<br>
<br>
The created CSV files can be found here: https://drive.google.com/drive/folders/1Ku0PFKlWstaLbY0ine2Q_LnbC5SLzctG?usp=sharing
<br>
## Workflow

- We chose the our data<br>
- We used basic pandas functions to familiarise ourselves with the data. (head(), shape, isnull().sum() ...)<br>
- Made some basic visualisations with tableau to see if there was anything obvious.<br>
- Merged the datframes with each other.<br>
- Checked the correlation of energy usage with different variables.<br>
- We then made:<br> 
-> a scatter plot and deleted the outliers.<br>
-> an OLS model and checked the statistical relevance.<br>

## Repository organisation

- Notebooks (Folder) :<br>
-> average_weekday_consumption.ipynb : calculate and plot average energy consumption by weekday<br>
-> concat_blocks.ipynb : look at half hourly meter readings for each household (NOT USED IN FINAL ANALYSIS)<br>
-> dataset_analysis_cleaning.ipynb : initial cleaning of original datasets downloaded from Kaggle<br>
-> linear_regression_visualisation.ipynb : look at energy consumption by ACORN group and which variables have the strongest correlation with energy consumption<br>
-> merge_dailydata_households_acorn.ipynb : merge daily_dataset.csv & informations_households.csv<br>
-> merge_weather-daily_data.ipynb: merge weather_daily_darksky.csv with daily_dataset.csv<br>
-> modified_Regression_model.ipynb : linear regression analysis<br>
- Tableau (Folder) :<br>
-> Tableau_merged_weather_Daily.twb : Tableau file with the graphs for the presentation.
- Presentation (Folder) :<br>
-> Contains final version of the presentation as a PDF file, along with presentation notes.<br>
- .gitignore file<br>
- README file<br>

## Results/findings

- Those with a higher income (ACORN-A) consume more energy on average than those with a lower income (ACORN-Q)
- Weekends saw the highest levels of energy consumption
- There’s a clear seasonal pattern, more energy consumption in colder months
- Negative correlation between the number of daylight hours and energy consumption
- Negative correlation between the average daily temperature and energy consumption (0.84 R-squared value)
- Carried out regression on the model (R-squared value = 0.68)
- Overall energy consumption in London during the time period shows a slight downward trend over time

## Potential improvements/future analysis

- Look further into potential outliers
- Exclude dates at the start of the testing period where the number of installed meters is small
- Dive deeper into consumer demographics
- Look at energy consumption by individual households
- Try quadratic regression to see if energy consumption increases in high temperatures
