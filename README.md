# NYC-TaxiDemandPrediction
----
### `Business Problem/Problem Statement:`
* For a given location in NYC, our goal is to predict number of pickups in that given location. Some location require more taxis at a particular time than other locations like schools, hospitals, offices etc. The prediction result can be transferred to the taxi drivers via Smartphone app, and they can subsequently move to locations where predicted pickups are high.
----
### `Objectives & Constraints:`
`Objectives:` 
* To predict number of pickups as accurately as possible for each region in an interval of 10min. 
* Breaking up whole New York City into regions, will help a loat.
* 10min interval is chosen because in NYC one can commute 1 mile in approximately 10 minutes given traffic is normal at that particular time.

`Constraints:`
* Latency given a location and current time of a taxi driver, as a taxi driver excepts to get predicted pickups in particular region and adjoining regions in few seconds. So, latency requirement is medium.

`Interpretability:`
* As long as taxi driver gets good prediction result, interpretability of the result can be ignored in some wasys. Taxi driver is not much interested in why they are getting this result. So, no interpretability required.

`Relative Errors:`
* Mean Absolute Percentage Error will be the relative error we will consider. 
* Let say predicted pickups for a particular location are 100, but actual pickups are 102,then percentage error will be 2% and Absolute error is 2. 
* Taxi driver will be more interested in the percentage error than absolute error. Let say in some region predicted pickups are 250, and if taxi driver knows that relative error is 10% then they will consider predicted result to be in range of 225 to 275, which is considerable.

`Goal:`
* To reduce the percentage error as low as possible.

`Source of Data:`
Data can be downloaded from here:
http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml. Here, we have used Jan- 2015 and Jan- 2016 data.
---
`Getting Started:`
* Start by downloading project and run "Taxi-Demand-Prediction-NYC.ipynb" file in ipython-notebook.

`Prerequisites:`
* Installed following softwares and libraries in your machine before running this project.
  - Python 3
  - Anaconda
  - Libraries:
  - Dask: Used to handle very large files.

i) pip3 install dask

i) pip3 install folium
folium: Used to plot maps using latitude and longitude.
ii) conda install -c conda-forge folium

i) pip3 install xgboost
ii) conda install -c conda-forge xgboost

i) pip install gpxpy
gpxpy: Used while we calculate the straight line distance between two (latitude, longitude) pairs in miles.

`Authors:`
* Mukesh Manral


