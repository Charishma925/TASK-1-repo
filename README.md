# TASK-1-repo
DATA CLEANING AND PREPROCESSING
Dataset used: Life Expectancy(WHO)
Description of dataset:The Global Health Observatory (GHO) data repository under World Health Organization (WHO) keeps track of the health status as well as many other related factors for all countries.
The datasets are made available to public for the purpose of health data analysis. The dataset related to life expectancy, health factors for 193 countries has been collected from the same
WHO data repository website and its corresponding economic data was collected from United Nation website.
The individual data files have been merged together into a single dataset. On initial visual inspection of the data showed some missing values. 
As the datasets were from WHO, we found no evident errors.
Missing data was handled in R software by using Missmap command. The result indicated that most of the missing data was for population, Hepatitis B and GDP.
The missing data were from less known countries like Vanuatu, Tonga, Togo,Cabo Verde etc.
Finding all data for these countries was difficult and hence, it was decided that we exclude these countries from the final model dataset. The final merged file(final dataset) consists of 22 Columns and 2938 rows which meant 20 predicting variables. 
All predicting variables was then divided into several broad categories:​Immunization related factors, Mortality factors, Economical factors and Social factors.
STEPS FOLLOWED TO CLEAN AND PREPROCESS THE DATASET
1.Import the LIFE EXPECTANCY dataset and explore basic info (nulls, data types).
2.Handle missing values using mean/median/imputation.
3.Convert categorical features into numerical using encoding.
4.Normalize/standardize the numerical features.
5.Visualize outliers using boxplots and remove them.
