# Air-Quality-Index Prediction using algorithms like linear, ridge, lasso, decision tree,random forest and XGBoost 

PROBLEM DESCRIPTION:
The aim of this project is to predict the air-quality index(PM 2.5 VALUE) based on the weather data which has 14 feautures like average temp.,atmospheric pressure etc.

DATA COLLLECTION:
The data is scrapped from website(https://en.tutiempo.net) using BeautifulSoup library. The data includes daily weather data from the year 2013 to 2018 for the city of bengaluru. Html_scripy.py file contains the code that retrieve the Html code from the website and Extract_combine.py scraps the data from the respective Html codes and combines them with the data stored in the AQI folder. AQI folder contains the target PM2.5 data in hourly format from the year 2013 to 2018. Plot_AQI converts the data stored in AQI in daily format so that it is compatible to combine with weather data. The final combined data is stored in Real_data folder.

To solve the task, I used various machine learning algorithms like linear, ridge, lasso, decision tree,random forest and XGBoost and Random Forest regressor gave the best results.

Outputs for different algorithms are stored in different .pkl files which can be used for further deployment of the project using services like heroku.

DATA DESCRIPTION:
Here is a brief description of the data extracted from web:

T	  Average Temperature (°C)                                                                                                                              
TM	Maximum temperature (°C)                                                                                                                               
Tm	Minimum temperature (°C)                                                                                                                               
SLP	Atmospheric pressure at sea level (hPa)                                                                                                                 
H	  Average relative humidity (%)                                                                                                                           
PP	Total rainfall and / or snowmelt (mm)                                                                                                                   
VV	Average visibility (Km)                                                                                                                                 
V	  Average wind speed (Km/h)                                                                                                                               
VM	Maximum sustained wind speed (Km/h)                                                                                                                     
VG	Maximum speed of wind (Km/h)                                                                                                                           
RA	Indicate if there was rain or drizzle (In the monthly average, total days it rained)                                                                   
SN	Snow indicator (In the monthly average, total days that snowed)                                                                                         
TS	Indicates whether there storm (In the monthly average, Total days with thunderstorm)                                                                   
FG	Indicates whether there was fog (In the monthly average, Total days with fog)
