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

For this project, we used several datasets from Kaggle on Energy consumption in london, weather a that time and Acorn groups. We downloaded the following datasets from Kaggle and used statistical analysis skills to analyze this dataset:<br>
<br>
- acorn_details.csv<br>
- daily_dataset.csv<br>
- weather_daily_darksky.csv<br>
- informations_households.csv<br>
<br>
The Datasets can be downloaded from the following link: https://www.kaggle.com/jeanmidev/smart-meters-in-london?select=daily_dataset.csv.gz


## Workflow

- First: We read the data into a DataFrame<br>
- Second: I used basic pandas functions to familiarise myself with the data. (head(), shape, isnull().sum() ...)<br>
- Deleted all unnecessary columns.<br>
- wrote function to find the columns with a absolute correlation of at least 0.6. (I found 6 colums)<br>
- I then made:<br> 
-> an OLS model all six Columns and checked the statistical relevance.<br>
-> an OLS model with four of the six Columns since they had the same unit and that way we could compare them between each other and check the statistical relevance. (Square feet)<br>
-> an OLS model all with only the column with the biggest corrolation and checked the statistical relevance

## Organization

In the repository you will find several files and a Folder:<br>
<br>
1 - Data (Folder) :<br>
-> Download_link.md : Has the link to download the data<br>
2 - Notebook (Folder) :<br>
-> Average_weekday_consumption.ipynb : Calculates and Plots the average weekday consumption<br>
-> Merge Weather-Daily_data.ipynb : Used to merge weather_daily_darksky.csv with daily_dataset.csv and export as daily_weather_merged.csv<br>
-> Modified_Regression_model.ipynb : Checking correlation from temperature and daytime with energy consumption and building an OLS-Model and scatterplot<br>
-> paul_dataset_analysis.ipynb :<br>
-> paul_linear_regression_visualisation.ipynb :<br>
-> paul_merge_dailydata_households_acorn.ipynb :<br>
3 - Tableau (Folder) :<br>
-> Tableau_merged_weather_Daily.twb : Tableau file with the graphs for the presentation.
4 - .gitignore : To not push everything.<br>
5 - README.md : That would be this beautiful file :P<br>
    
## Links
[Repository](https://github.com/fctonio/Smart-meters-analysis)
