# Doctors-pharmacy-project
In this project I had a dataset of ~6000 doctors addresses and a dataset of ~500 pharmacy addresses in Paris. The goal was to find for each doctor what pharmacy was the closest by distance wise so that they could be recommended for the customers. 

There were two major steps in this project:
1. Quering the Google maps API to get the latitude and longitude for each of the adresses as to facilitate distance calculation.
2. Create a distance function based on pythagorean formula and applying this in a nested loop, so that for each doctor all distances to each pharmacy are calculated and than the minimum value is chosen and this doctor - pharmacy pair is than appended to an empty dataframe. 

Step 1 was all done in R with the ggmap package (note, my api keys are removed from the data).
Step 2 was tried in R but for some reason the loops failed so finally it was coded in python which worked out.
