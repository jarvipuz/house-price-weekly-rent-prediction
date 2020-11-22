### COMP257/ITEC657 Group Project
## Project Title: Housing Price and Weekly Rent Prediction
#### Group: ITEC _ Pract _ 03(Tue 7pm) _ Group B
#### Group Members:
* Abdul Sattar Mohammed - 45830541
* Jan Arvin Lapuz - 45758891
* Jerome Roosan - 45999589
* Le Van Nguyen - 45817006


## Overview

The house prices as well as weekly rent in Sydney and nearby regions in NSW are increasing day by day. Although there is an obvious growth in the economy that drives the growth, there are many other features affecting the house prices and weekly rent in some areas as compared to others. This includes factors such as the demographic of certain locality, transportation facilities nighttime lights etc.

So the main goal of the project is to understand,
* **How are the demographics, transportation and nighttime lights relate to house price and weekly rents?**
* **What are the best features that help predict the house price and weekly rents?**


## Delivery 

The underlying analysis and experimentation were recorded in a collection of Jupyter notebooks. The team members divided the tasks among themselves in differnet stages from collecting the data sets to different analysis methods, and combined the notebooks. Based on the analysis, a project report is made along with a few slides for the project presentation.


## Project Activities

### Defining the data

We downloaded the details of population demographics per LGA from the 2016 Census Data Packs (Ref link 1). Similarly, we got the transportation details from an API managed by Transport for NSW website (Ref link 2) and nightime lights data were downloaded from  Defence Meteorological Satellite Program database by the National Oceanic and Atmospheric Association (NOAA) (Ref link 3). All these were datasets containing the predictor variables. The reponse datasets are based on the house sales and weekly rent data downloaded from the Family & Community Services website (Ref link 4).

The census data was developed based on the Local Government Area (LGA). So we used LGA as the unit of analysis and the merging criteria for all of the datasets. A LGA lookup dataset was created with the suburb names and used it to merge all datasets in the preprocessing stage and prepare a single dataset for further analysis. We have done some preprocessing of the data to create a simpler dataset with the relevent information. Python notebooks are used for the data processing which helped a lot in getting the data cleansing done easily.


### Analysing the data

We have used various Python packages in the analysis such as:
* Pandas
* NumPy
* Matplotlib
* seaborn
* OSGeo
* GeoPandas
* GridSearchCV
* scikit-learn
* rasterio

We have plotted the data sets to check the relationships and used regression analysis techniques for mapping the data from different datasets. Regression analysis techniques such as Linear Regression and Decision Tree Regressor were carried out to find which regression technique is best for generating model with highest accuracy score. These analysis were done on rent and sales data against each of the main variables.


### Selecting the best predictors

Along with the individual analysis of each feature with the rent and sales data, we have used recursive feature elimination technique to find the best features that can be used to predict the data with higher accuracy.


### Project Report

The project report is also developed using notebook. **Housing Price and Weekly Rent Prediction Final Report.ipynb** has been prepared detailing the preprocessing and analysis techniques with some visual and statistical outputs.


## Folder Structure
This repository is organised as follows:
* Data/ - folder containing all the relevant datasets that were used in the analysis
* Files/ - folder containing the graphics used in the final report
* group presentation/ - folder containing the presentation deck summarising the results of the analysis to be presented during the practical class of Data Science Week 13
* Data_Analysis_* - Jupyter notebook containing details of the analysis conducted and who prepared the file
* Data_Preprocessing_* - Jupyter notebook containing data compilation and manipulation codes to come up with the final cleaned dataset
* Housing Price and Weekly Rent Prediction Final Report - Jupyter notebook summarising the project from the motivation, data collection and data analysis


## References

* Ref link 1: Census Dataset and Shapefiles [https://datapacks.censusdata.abs.gov.au/datapacks/]
* Ref link 2: Transportation Points [https://opendata.transport.nsw.gov.au/node/334/exploreapi#!/gtfs/GetSydPubTransGTFS]
* Ref link 3: Nighttime Lights [https://ngdc.noaa.gov/eog/viirs/download_dnb_composites.html]
* Ref link 4: House Sales and Weekly Rent [https://www.facs.nsw.gov.au/resources/statistics/rent-and-sales/dashboard]
