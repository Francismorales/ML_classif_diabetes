# Machine Learning Classification System
Machine Learning classification system to determine the level of diabetes in the population of US counties.


The ML classification model selected for the classification problem was a SVM. I wrote a blog post explaining the evaluation process I followed to select my model: 
**Multi class ML Model Evaluation**: https://medium.com/analytics-vidhya/multi-class-ml-models-evaluation-103c9fdadb41


### ABOUT THE DATASET
A total of **820 samples** of data with **50 variables** containing US counties economic features, demographics, geographic coordinates, weather components & food access were used for the study. Labels were defined as High/Medium/Low based on the percentages of diabetes of each county.

![alt text](https://github.com/Francismorales/ML_classif_diabetes/blob/master/images/Label_Distribution2.PNG)

Data was extracted by using web scraping, by connecting to different APIs and by downloading datasets directly from a webpage. 

List of data sources with links:

1. US Census Bureau: API - https://api.census.gov/data/2018/acs/acs1.json?get=[VARIABLESHERE]&for=county:*
2. US Department of Agriculture:https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data/
3. Centers for Decease Control and Prevention: https://gis.cdc.gov/grasp/diabetes/DiabetesAtlas.html#
4. Zillow: https://www.zillow.com/research/data/
5. Menuism: https://www.menuism.com/
6. National Centers for Environmental Information: https://www.ncdc.noaa.gov/
7. Wikipedia: https://en.wikipedia.org/wiki/User:Michael_J/County_table

## FILES & FOLDERS

#### ML_classifDiabetes.ipynb

This is the main jupyter notebook. Below are the sections within the notebook: 

      1. Libraries & Functions
      2. Data Engineering
      2. Exploratory Data Analysis
      3. Machine Learning classification algorithms: 
            - Random Forests 
            - SVM 
            - K-NN 
            - AdaBoost and Gradient Boosting classifiers
      4. Conclusion 

#### MLDiabetes_WebScraping.ipynb

This notebook has the step-by-step Web Scrapping process used to collect McDonald's, weather & county coordinates data. 
**You do not have to run this notebook to replicate the results of the main notebook as the web scrapped data was saved to the DATA folder**

For the McDonald's restaurant count, the web scrapping data quality was checked using Google Maps: Places API. I wrote a couple of blog posts explaining this process: 

**Web Scraping:**  https://medium.com/swlh/web-scraping-for-data-collection-d41c6505235d

**Google Maps: Places API:** https://medium.com/swlh/google-maps-places-api-28b8fdf28082



#### Folder: DATA
Folder with files dowloaded from data sources. This folder is called from the **ML_classifDiabetes.ipynb**, therefore you need to make sure to have this folder and all its files saved to the directory were you run your jupyter notebook. 

Data files are stored on this folder. The data was obtained from multiple sources using Web scrapping, connecting to APIs, and downloading it directly from websites. 

ML_classifDiabetes.ipynb has an explanation of the data source, data dowload method 


#### Folder: Shapefile_USA
This folder has the shapefiles  to plot data in the US map. 





