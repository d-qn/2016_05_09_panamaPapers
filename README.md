# The Panama Papers intermediaries

R script used to analyse [ICIJ's offshore leaks database](https://offshoreleaks.icij.org)

It uses the csv file available [here](https://cloudfront-files-1.publicintegrity.org/offshoreleaks/data-csv.zip#_ga=1.76380693.1812329309.1462825617) of all intermediaries in the offshore leaks database.

The R markdown file *01_explore.Rmd* will create a series of interactive map based on leaflet.js. Please note that there are many dependencies to that script for now, but it should give an idea 

## Method

1. [csv file of all intermediaries](https://cloudfront-files-1.publicintegrity.org/offshoreleaks/data-csv.zip#_ga=1.76380693.1812329309.1462825617) (in the folder *data*)
2. The csv data file contains intermediaries from the offshore leaks and the Panama Papers. The data was subset to get only Panama Papers' intermediaries -> 14110 entries
3. Some intermediaries have multiple addresses and countries. Because I was interested to map all intermediaries, some entries were duplicated in order to have only one address/country per entry. This means that the 14110 intermediaries led to 24372 locations. 
4. The countries of these 24372 locations were displayed on a map. Please not that 1929 locations could not be mapped. 