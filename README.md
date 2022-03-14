# DE200-Project

This repository contains all of the files for our DE 200 project at Northwestern University. Here are their explanations in the order of their creation



InjuryToCSV.py
This is the python script that was written to scrape all of the injury data from the NFL's offical website, https://www.nfl.com/injuries/.
The URL takes in the year and regular season week like so: https://www.nfl.com/injuries/league/2001/REG1. We scraped all of the regular season injury reports
from 2001 to now and stored them into a csv file

InjuryDataDirty.csv
This is the data we scraped without doing any cleaning. Almost 64000 entries

CsvDataClean.py
This script was written to clean the data using pandas. Directional words like "right" and "left" were removed. Noninjuries were removed. 
Injuries that needed to be grouped together were grouped together. Position labels were modernized (NT for nose tackles used to be used
instead of DT sometimes, for example). Some players were listed for multiple injuries so these were split. Some entries did not have
a value for injury, so they were removed. Specific injuries that did not fit into a category were put into an "Other" category.

FootballInjuries.csv
This is data after being cleaned from the previous script. About 15000 entries
