# Epidemic_Detection_System 
This project aims to collect data from local hospitals like number of patients admitted per day. It the aims to find breakout of infectious diseases in different locations using the data on hospitalizations.

The ipynb files can be run on Anaconda. You can also copy the code and run it in a .py file. Either way make sure you ahve the following libraries installed.
1)numpy
2)urllib

There are three core scipts

1)Dataset Generator - This generates the dataset of patients with some random symptoms and determines if they survive or not. This is set for a particular locality with a certain random number of patients being generated for each date between the start date and the end date.  On top of this an epidemic can be simulated for each locality. You can consider each locality like the area around a hospital or a taluk. All this data is stored in a newly created folder Hospitals. 

2)Data_organisation_hospital_side - This compiles the data from these hospitals to a single file 'Compiled.txt' This contains the growth parameters and percentage of occupancy of hospitals which are also calculated in this file.

3)Data_Analysis_Central - This script takes data from the compiled file to display it in a map of Kerala. This can be modified to any state or country if you have the geojson file available for the particular entitiy.

Notes on the code:

Data_organisation_hospital_side.ipynb runs based on current computer date. So I recommend you to set the date correctly and provide end date as your computer date+1 day as the last day is not generated in view of effects from incomplete data if the code is deployed in a hospital.

The last script modifies Keralataluk.js file so that the parameters are displayed when index.html is opened. Make sure the folder leaflet is also downloaded when you run the program as it contains an important plugin required for the map to work.


I would also like to thank the creaters of the plugin Leaflet, Mapbox and OpenStreetMap whose data and plugins were of great help in this project.
I am also deeply thankful for the work of Sajjad Anwar in making geojson maps of India which were of great use in this project.

