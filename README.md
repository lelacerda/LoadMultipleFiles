# Loading multiple files using Python

## Overview
Loading one single file using Pandas library in Python is pretty straigh forward. But what happens if you need to load several files and concatenate them into only one file for analysis? 

Python has a module called [glob](https://docs.python.org/3/library/glob.html#module-glob) that allows you to load multiple files located in the same directory, assigning them to a single object. Then it is possible to read and concatenate all files stored into this object into a single pandas dataframe using a for loop command. The newly concatenated table can have a new index to take into account all rows added excluding the original indexes from each table.


## Data
I used historical weather data from [Canada Government website](https://climate.weather.gc.ca/historical_data/search_historic_data_e.html). I chose daily weather data from Halifax Stanfield Airport Station from 1961 to 2022.

## Procedure

All files downloaded had the same file name structure e.g. 'en_climate_daily_NS_8202250_1960_P1D.csv'. As the only change in file name for these datasets is the year, it is possible to change the file name using 'en_climate_daily_NS_*.csv' when using the glob code.

Click [here](https://github.com/lelacerda/LoadMultipleFiles/blob/main/Load_Multiple_Files.ipynb) to see how do it.
