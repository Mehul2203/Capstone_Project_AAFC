# Exploring Optimal Machine Learning Models for Predicting Crop Yield at Township Level

The project aims to explore optimal machine learning models for predicting crop yield based on growing patterns at the township level using the Python programming language with its various libraries and packages for applying Deep Learning methods and algorithms.

## Team Members

- Navdeep Singh Saini: Data Science Enthusiast with the technical and business expertise along with the Analytical acumen to translate real world customer problems into data-driven decisions
- Mehul Bhargava: Data Science professional with strong academia and experience performing end-to-end data analysis from extracting raw data to generating dashboards and building predictive models. Strong communicator and passionate about problem solving.
- Mayukha Bheemavarapu: Data Scientist experienced in the domains of Ecommerce, Retail and BFSI industries with specialization in Ad/Web Analytics. 
- Val Veeramani: Analyst with a strong business acumen who loves creating intriguing data visualizations!

## INTRODUCTION

Crop yield and production are crucial to meet the demands of millions in this country. Apart from that, one of the most important aspects is to increase exports, and to achieve that, prior information regarding the yield is highly significant, especially for the decision makers who can further formulate the export policies based on the results generated related to the crop yield forecast. Due to crops being one of the 4 key sectors managed by Agri-Food Canada, it is in our best interest to make sure that this sector is performing to its highest capacity.  Not to mention that there are several millions of individuals counting on its sustained performance, we are tasked with ensuring that we are able to keep up with the demand of them in the coming years and the future. As AAFC works to grow exports, while providing leadership in the expansion and development of a competitive, innovative, and sustainable Canadian agriculture and agri-food sector, the project is quite essential to come up with data driven planning with regards to agricultural production.

## AIMS & OBJECTIVES

We seek to test Machine Learning (ML) methods for predicting crop yield at township level. Currently, crop yield prediction and forecasting is accomplished using the Canadian Crop Yield Forecaster where weekly low resolution (~1km) NDVI values and daily agrometeorological variables from unevenly distributed climate stations are used in a blended model which uses statistical and biophysical modules (Newlands et al. 2014). A number of issues arise when statistical based models are used to predict crop yield such as multicollinearity among predictor variables and lack of plausible scientific explanation for  some predictor variables that are selected in some experiments (inference).Studies with ML algorithms have shown that predictions can be made without making any prior assumptions about the relationship between the response and predictor variables (You et al., 2017, Cai et al., 2019, Yang et al., 2019). Using the Canadian Prairie domain as the study area, we seek to test the following algorithms (or better ones) in the prediction of canola, spring wheat and barley; XGBoost and Lasso and compare results with observed values. We propose to use  cloud-based resources such as Google Earth Engine for processing large amounts of data without physically downloading the data. This will allow the use of complicated procedures such as Deep Learning libraries for training the models. 

## DATASET DESCRIPTION

### Crop Yield Data:
AAFC has access to crop yield data provided by provincial governments of Alberta, Saskatchewan and Manitoba via an memorandum of understanding (MOU). Originally at quarter section  level, these data sets have been rescaled to township level using geostatistical techniques. These data sets will be used as observations for training the models.

### Earth Observation Predictor Variables:

AAFC scientists and partners have assembled ground and satellite derived predictor variables for improving the crop yield prediction skill at finer scale. Examples include the Normalized Difference Vegetation Index (NDVI) from Synthetic Aperture Radar (SAR) and optical sensors, surface soil moisture from active and passive microwave sensors, the evaporative stress index from thermal-optical data, leaf area index from Sentinel-2 and high resolution modelled weather data sets from the Canadian Meteorological Centre at 2.5km and 10km. These data sets have been aggregated at township level for at least 20 years. Other data sets include value added variables derived from intermediate models such as the Versatile Soil Moisture Budget (VSMM) from which soil moisture and crop stress index are calculated and used as input in the crop yield prediction models. Heat related indices such as Growing degree days and stress days are equally available. All data sets are organized as tables and tagged to townships by crop type (using crop density maps).


## ACKNOWLEDGEMENTS & REFERENCES 

Luca Sartore, Arthur N. Rosales, David M. Johnson, Clifford H. Spiegelman, Assessing machine leaning algorithms on crop yield forecasts using functional covariates derived from remotely sensed data, Computers and Electronics in Agriculture, Volume 194, 2022, 106704, ISSN 0168-1699.

Huiren Tian, Pengxin Wang, Kevin Tansey, Jingqi Zhang, Shuyu Zhang, Hongmei Li,
An LSTM neural network for improving wheat yield estimates by integrating remote sensing data and meteorological data in the Guanzhong Plain, PR China, Agricultural and Forest Meteorology, Volume 310, 2021, 108629, ISSN 0168-1923.

Saeed, Umer & Dempewolf, Jan & Becker-Reshef, Inbal & Khan, Ahmad & Ahmad, Ashfaq & Wajid, Syed. (2017). Forecasting wheat yield from weather data and MODIS NDVI using Random Forests for Punjab province, Pakistan. International Journal of Remote Sensing. 38. 4831-4854. 10.1080/01431161.2017.1323282.

Aston Chipanshi, Yinsuo Zhang, Louis Kouadio, Nathaniel Newlands, Andrew Davidson, Harvey Hill, Richard Warren, Budong Qian, Bahram Daneshfar, Frederic Bedard, Gordon Reichert, Evaluation of the Integrated Canadian Crop Yield Forecaster (ICCYF) model for in-season prediction of crop yield across the Canadian agricultural landscape, Agricultural and Forest Meteorology, Volume 206, 2015, Pages 137-150, ISSN 0168-1923
