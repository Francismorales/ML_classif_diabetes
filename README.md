# ML_classif_diabetes
Machine Learning classification system to determine the level of diabetes in the population of US counties.

### Data Sources
A total of **820 samples** of data with **50 variables** containing US counties economic features, demographics, geographic coordinates, weather components & food access were used for the study. Labels were defined as High/Medium/Low based on the percentages of diabetes of each county.

Data was extracted by using web scraping, by connecting to different APIs and by downloading datasets directly from a webpage. 

1. US Census Bureau: API - https://api.census.gov/data/2018/acs/acs1.json?get=[VARIABLESHERE]&for=county:*
2. US Department of Agriculture:https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data/
3. Centers for Decease Control and Prevention: https://gis.cdc.gov/grasp/diabetes/DiabetesAtlas.html#
4. Zillow: https://www.zillow.com/research/data/
5. Menuism: https://www.menuism.com/
6. National Centers for Environmental Information: https://www.ncdc.noaa.gov/
7. Wikipedia: https://en.wikipedia.org/wiki/User:Michael_J/County_table

![alt text](https://github.com/Francismorales/ML_classif_diabetes/master/images/Label%20Distribution.png?raw=true)

## **Folders**:
- **DATA**: Data files are stored on this folder. The data was obtained from multiple sources using Web scrapping, connecting to APIs, and downloading it directly from websites. 

ML_classifDiabetes.ipynb has an explanation of the data source, data dowload method 


## Repository Files:
- **ML_classifDiabetes.ipynb** : Main jupyter notebook containing:

      - Data Engineering
      - Exploratory Data Analysis
      - Machine Learning classification algorithms: Random Forests, SVM, K-NN, AdaBoost and Gradient Boosting classifiers
      - Results summary 


