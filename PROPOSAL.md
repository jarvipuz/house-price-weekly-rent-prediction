Housing Price and Weekly Rent Prediction - Sydney
===

*ITEC657 Data Science Project Proposal*

Van Nguyen (45817006), Jan Lapuz (45758891), Abdul Sattar (45830541), Jerome Roosan (45999589)

# Summary
Housing sales and rent price prediction is not a new subject for doing data analysis. However, there are many variables affecting property pricing and not many of them make use of characteristics about transportation, wealth, demographic information, transportation stops and nightlights information. Our main target is to be able to predict housing price and weekly rent on each of New South Wales' Local Government Areas by investigating those indicators.

## Goals
The main goal of the project is to create a model to predict housing price and weekly rent for each Local Government Area and of the NSW region. Other areas that we will explore are:
* Check which transportation and demographic characteristics are most relevant in predicting house pricing and weekly rents
* Examine the effects of introducing remote sensing data, such as nighttime lights, into the model
* Explore different regression techniques and find out which one provides a better prediction

## Datasets
The analysis will make use of 4 main datasets: housing sales and weekly rent figures from NSW Department of Family and Community Services, transportation information from Transport for NSW Open Data Hub, demographic characteristics from the Census and Population Housing which can be obtained by using the Census Data Packs of the Australian Bureau of Statistics and nighttime satellite imagery from National Oceanic and Atmospheric Association (NOAA).

The NSW Department of Family and Community Services releases quarterly reports on housing and rent prices in the NSW region containing summary statistics on prices such as 1st quartile, median, 3rd quartile and mean by Local Government Area (LGA) and postcode. The summary statistics are also broken down by dwelling type and, for weekly rent prices, number of bedrooms.

The Transport for NSW Open Data site maintains an API that provides different transportation stops within NSW. This includes all bus stops, coach stops, train stations, light rail stations and wharfs. The dataset is in the form of a text file that has been converted to a map using the coordinate system provided in the file.

Demographic characteristics, such as population and income data, for each LGA may be obtained through the Australian Bureau of Statistics Census Data Packs site. The tool uses the information collected from the Census of Population and Housing and provides aggregate values based on different characteristics. The 2006, 2011 and 2016 census data is available but more recent data has less granular view of the entire dataset.

The NOAA collects daily information on the amount of light generated at night and processes it to develop an image that estimates the amount of light at night. The image contains a matrix of pixels with each pixel representing a 500 meter by 500-meter area. Nighttime lights is available for almost every surface of the earth and summary statistics can be extracted for each LGA of NSW region.

Python packages to be used in the analysis:
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Osgeo
* Geopandas
* GridSearchCV
* SciKit-learn
* rasterio

# Analysis Techniques
We will be using regression analysis techniques for mapping the data from different datasets. Regression analysis techniques such as Linear Regression and Decision Tree Regressor will be carried out to find which regression technique is best for generating model with highest accuracy score. We will also be individually checking all the "variables" against "Rent & Sales variables" to pick up and finalize the variables along with RFE and predict our final results. 

# Project Plan
* Milestone #1 - end of Week 8:
	* Resolve all works relating to dataset usability
	* Finish data cleaning, joining and converting if needed

* Milestone #2  - end of Week 9:
	* Finish exploring dataset:
		* Analyse any trend and correlation
	* Decide which algorithms to use

* Milestone #3 - end of week 10:
	* Finish modelling the data
	* Validating the model

* Milestone #4 - end of Week 12:
	* Draw conclusion about housing price prediction
	* Finalize needed documents
	* Finish preparation for the presentation
