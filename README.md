# Analyzing-Continuous-vs-Gravimetric-PM2.5-Monitor-Concentrations
>An analysis of concentration differences between collocated Gravimetric and Continuous PM2.5 monitors across the United States using data from the U.S. EPA's Air Quality System (AQS). Various parameters will be explored that could help explain the differences (e.g., temperature) and a ML model is used to predict differences based on these factors.
>In the U.S. EPA National PM2.5 monitoring program, the use of Federal Equivalent Method (FEM) continuous monitors continues to increase in comparison to the Federal Reference Method (FRM) gravimetric monitors. There exists a known bias in 24-hour ambient PM2.5 concentrations between these two methods. Monitoring agencies need to understand these biases, its causes, and determine if PM2.5 continuous monitoring is appropriate for their network. This project aims to investigate these biases, determine the contributing factors, and attempt to predict FRM concentrations based on collocated FEM concentrations and these other factors.
> A blog post summarizing these results can be found on Medium: https://medium.com/@brannonseay/concentration-analysis-between-epas-continuous-and-gravimetric-pm2-5-monitor-a98bb8ee9cae

# Installation needed
> Developed on Python 3.8.5. Relevant packages used include:
>> Pandas v1.2.1
>> Numpy v1.19.2
>> Requests 2.25.1
>> Meteostat v 1.5.10 (to install: pip install meteostat)

# Files for project
> The Jupyter Notebook (cont_v_grav_pm25_monitors.ipynb) is where all data gathering, assessing, analyzing, etc. occurred.
> I've also saved the following .csv files, which include critical datasets gathered and cleaned throughout the process.
>> monitor_data.csv (provides monitoring site specific information; pulled from EPA's AQS API)
>> daily_data_2016_20.csv (provides daily concentration data from 2016-2020; also pulled from EPA's AQS API)
>> met_data_2016_20.csv (meteorological data from every monitoring site/date; pulled through Meteostat python library)
>> methods_all.csv (provides all epa method codes; downloadable from https://aqs.epa.gov/aqsweb/documents/codetables/methods_all.html)
>> frm_vs_fem.csv (this is the cleaned up dataset including info from each of the above files. This is the dataset analyzed in depth and ML implemented)

# Licensing, Authors, Acknowledgements
> All air quality data freely available through EPA's AQS.
