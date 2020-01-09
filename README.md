# Vehicle Safety Ratings
In this project I will investigate the crash reports and try to find which types of vehicles (body type/make/model) are safer. 
# Motivation
I allow my analytical skills to help my decision making for possible future vehicle purchases. When deciding a car to buy, the safety is always a major issue. As a matter of fact, it may be the most important feature.

There are [safety rankings](https://www.nhtsa.gov/ratings) available from NHTSA (National Highway Traffic Administration), but it is created based on the test results. These test crashes happen in a laboratory environment which covers only certain types of crash conditions.

What I want to see is what is happening in real world. Hence, I look answer from **accidents reported in _2016, 2017 and 2018_, in US.** 

# Data Question
There is a [similar work](https://www.iihs.org/api/datastoredocument/status-report/pdf/52/3) from a nonprofit organization, The Insurance Institute for Highway Safety (IIHS) about **_death rates_** by make and model. This report shows the fatality rate of vehicles.

I want to look the whole crash data instead of fatal crashes. Hence the question of this project is more general: Which make, model vehicles are safer? 

# Data Preparation
The main source of my data is NHTSA and the big part of it is csv file. However, since one of the file for 2018 is not released yet, I pulled the vin decoding data from API.

**Data Sources:**
* [Accidents & vehicles](ftp://ftp.nhtsa.dot.gov/) : ftp://ftp.nhtsa.dot.gov/
* [VIN decode API](https://vpic.nhtsa.dot.gov/api/)
* [Car features and MSRP](https://www.kaggle.com/CooperUnion/cardataset/data)

**Data Manipulation:**

![alt text](https://github.com/ssimseksefa/Vehicle-Safety-Ratings/raw/master/damage_calculation_steps.png)

![alt text](https://github.com/ssimseksefa/Vehicle-Safety-Ratings/raw/master/safety_rate_calculation_steps.png)

# Results
Here is the [interactive dashboards](https://public.tableau.com/profile/sefa4601#!/vizhome/vehicle_safety_1/VehicleSafetyRatings) which you can find your next car.

# Future work
This analysis is made by crash reports only. So, I created safety rating from the results of crashes happened. However, many vehicles have safety features which may prevent the accident. If there is all registered vehicles data available, I also want to see pre-caution ratings for vehicles.
