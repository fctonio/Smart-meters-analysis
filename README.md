<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Statistical-Analysis-Project
*Paul Musco, Mayowa Akinyele and Anton Neike*

*Data-ber-08-20, Berlin & 16/09/2020*

## Content
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

## Project Description

The goal of this project is to create and interprete different types of visualizations using real world data as well as statistical analysis. For this project we worked in a group of three people and had to choose our own subject and data. The goal is to hold a presentation of 5 minutes at the end of the week and present our finding in a way anyone could understand.

## Dataset

For this project, we used several datasets from Kaggle looking at energy consumption in London, weather conditions over the same period and Acorn groups. We downloaded the following datasets from Kaggle and used statistical analysis skills to analyze this dataset:<br>
<br>
- acorn_details.csv<br>
- daily_dataset.csv<br>
- weather_daily_darksky.csv<br>
- informations_households.csv<br>
<br>
The Datasets can be downloaded from the following link: https://www.kaggle.com/jeanmidev/smart-meters-in-london

## Workflow

- We chose the our data<br>
- We used basic pandas functions to familiarise ourself with the data. (head(), shape, isnull().sum() ...)<br>
- Made some basic visualisation with tableau to see if their is anything obvious.<br>
- Merged the Datframes with each other.<br>
- Checked the Corrolation of energy usage with different variables.<br>
- We then made:<br> 
-> a scatter plot and deleted the outliers.<br>
-> an OLS model and checked the statistical relevance.<br>

## Organization

In the repository you will find several files and a Folder:<br>
<br>
- Data (Folder) :<br>
-> Download_link.md : Has the link to download the data<br>
- Notebook (Folder) :<br>
-> Average_weekday_consumption.ipynb : Calculates and Plots the average weekday consumption<br>
-> Concat_blocks.ipynb : <br>
-> Merge_weather-daily_data.ipynb: Used to merge weather_daily_darksky.csv with daily_dataset.csv and export as daily_weather_merged.csv<br>
-> Linear_regression_visualisation.ipynb : Looks into potential correlation between energy consumption and consumer demographics<br>
-> Dataset_analysis_cleaning.ipynb : initial cleaning of the original datasets<br>
-> Merge_dailydata_households_acorn.ipynb : merges 3 of the datasets to enable analysis of patterns/connections between them<br>
-> Modified_Regression_model.ipynb : Checking correlation from temperature and daytime with energy consumption and building an OLS-Model and scatterplot<br>
- Tableau (Folder) :<br>
-> Tableau_merged_weather_Daily.twb : Tableau file with the graphs for the presentation.
- .gitignore : To not push everything.<br>
- README.md : That would be this beautiful file :P<br>

## Potential improvements/future analysis

- Look further into potential outliers
- Exclude dates at the start of the testing period where the number of installed meters is small
- Dive deeper into consumer demographics
- Look at energy consumption by individual households
    
## Links
[Repository](https://github.com/fctonio/Smart-meters-analysis)
