# Final_Project_BigData, Marzia Tamanna
My final project is developed for the analysis of a dataset, including analysis of hydrological data and a ~1000 word paper on my analysis (focusing on methods and results). 

Initially I have used Gitbash for the following two steps.

First step:Data is downloaded by the following command in Gitbash

curl https://waterdata.usgs.gov/nwis/dv?referred_module=sw&search_site_no=01435000&search_site_no_match_type=exact&state_cd=ny&site_tp_cd=ST&index_pmcode_00060=1&group_key=NONE&sitefile_output_format=rdb&column_name=agency_cd&column_name=site_no&column_name=station_nm&range_selection=date_range&begin_date=2012-01-01&end_date=2016-12-31&format=rdb&date_format=YYYY-MM-DD&rdb_compression=value&list_of_search_criteria=state_cd%2Csearch_site_no%2Csite_tp_cd%2Crealtime_parameter_selection >usgs.csv

Second step:removing the lines starting with '#' by the following command in Gitbash

grep -v '^#'

For the rest of the analysis I have used R markdown for this project. Try1_FinalProject.Rmd starts directly from loading the downloaded data from data_streamflow_Neversink.csv file. The output of my project is Try1_FinalProject.pdf file. I have installed the following packages for my analysis.

install.packages("knitr")
install.packages("gridExtra")
install.packages("lubridate")
install.packages("ggplot2")
install.packages("scales")




