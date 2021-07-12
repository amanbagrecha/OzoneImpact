## Project for the course Geographic Information Systems (GIS) Specialization
The final course project to identify the impact of ozone in california 
## Hypothesis 
> There is no relation between ozone and income.
> There is a positive relation between ozone and elevation

In this analysis case study, the method followed was that initially I made a copy of the files so that i can try out certain things without any fear. then looked all the tables and primary and foreign keys and how they are correlated. 
I then took the ozone value to 'air quality table' and elevation values to 'air quality table'.
In income table, I first made a ozone raster using tins and created zonal stats based on census tract data and plotted the graph
steps taken
- join operation on air quality to ozone averages, which resulted in 187 records left
- extract by zonal statistics for table for elevation data to point ( air monitoring stations)
- created tin using 'create tin' from air quality table
- created raster from tin having cell size of 30 m
- used zonal statistics to include ozone data to census tract based data
- dissolved census tract based on block id
- classified (coloured) the dissolved data into 6 subs, with equal interval classification
- created graphs as asked to
- made 3 data frames, one for reference, one for map, one for graphs

## results: hypothesis was correct
> we see a positve trend with ozone and elevation. while there does not seem to be any relation between income and ozone concentration. what could be tested is certain other parameters such as air pollution which might significantly effect the ozone level at that station.
