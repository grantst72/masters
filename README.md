# masters project

This github account is used to securely save my code and so it can be accessed by my tutor if required. The aim of my project is to understand how changes in wildfire distribution over the savannahs of the Central African Republic is affecting vegetation structure. This will be done by analysing MODIS timeseries data along with the newer ICESat-2 satellite products. Please note: The data itself (~ 650GB) is not uploaded onto this account so running the scripts will produce an error.

For anyone interested in understanding this code:
  - comparing_NDVI: for loops through all burned area data products and creates an array for all pixels showing burn frequency. This is used to   categorise regions into low/ moderately low/ moderately high / high frequency burned area regions. I then split vegetation indices data (NDVI) depending on these regions so I can then analyse the differences between them.

## Project progress (08/12/20)

MODIS
I have downloaded all my MODIS Burned Area data onto my hard drive and have made significant progress in analysing it in python. The key thing to achieve was to categorise burned area frequency which i have managed to do in MODIS_Burned_Area_Clean.ipynb. To do this I  created a blank 2400*2400 array and for looped through all the MODIS files for that tile and added 1 every time it each pixel burned (monthly files over 19 years). This was then displayed as a colormap - shown at the bottom of the file. 

The next step is to compare this to the Vegetation Indices (currently being downloaded). I have made progress on the test run comparing it to a single VI file (TEST_comparing_NDVI.ipynb). There is one line causing me a problem but I expect to be able to overcome that shortly.


ICESat-2
I have been able to visualise an example of the ATL08 mean canopy height data. I did this over the summer but this has taken the backseat while I focus on the MODIS data. My next step for this is a relatively complex one as I need to plot this data on a per photon basis. I have the equations to do this, but I expect it to take a fair amount of work. I aim to get this complete over the christmas break as this would leave me in a strong positon to analyse the data when I return.

I have also got other python projects I am doing in my own time although I haven't uploaded these to github yet.
