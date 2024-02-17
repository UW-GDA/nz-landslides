# NZLandslides

Paul added this... and now Luis added this... and Alan added this!


## Project Title:  

Ground Changes after Coseismic landslides in Kaikoura New Zealand

## Name(s) of individual or team members: 

Luis Angel Guerrero Hoyos, Paul Morgan, Alan Viola

## Short 1-2 sentence summary: 

This project aims to measure and describe the factors that affected ground changes after coseismic landslides in Kaikoura, New Zealand. 

## Some introductory background information: 

On 14 November 2016, the region surrounding Kaikoura, New Zealand, experienced a M7.8 earthquake which triggered over 10,000 landslides. The modes of landsliding were diverse, including shallow, soil slides; rock avalanches and rock falls; and massive, deep-seated rotational slumps (Massey et al., 2018). Extensive mapping of the landslides triggered by the November 2016 earthquake has been undertaken by the New Zealand Institute of Geological and Nuclear Sciences (GNS).

Over the years, the GNS has done LiDAR and UAV - SfM surveys in the area that will serve as the main dataset to develop the project. The main goal is to track ground changes after the coseismic landslides, see how they’ve progressed over time, and find geospatial correlations between ground changes. We will focus on the LIDAR dataset collected by GNS between 2016 and 2019 and use the difference maps technique to identify the potential movements.


## Problem statement, question(s) and/or objective(s)

- How have ground changes progressed over time in the Keikoura region?
- How do properties like vegetation, slope, aspect ratio, and position relative to ridges and valleys affect ground changes after landslides?

## Datasets you will use (with links, if available)

Three Lidar DTMs from New Zealand Institute of Geological and Nuclear Sciences (GNS)
Landslide inventory polygon from GNS
Landsat imagery
Planet labs imagery (hopeful)
Global SRTM DEM


## Tools/packages you’ll use (with links)
Geopandas
Rasterio
rioxarray
numpy
matplotlib



## Planned methodology/approach

For a small subset study area in the Kaikoura coast range we plan to compile several datasets to analyze what happens to landslides after they occur. We will gather several separate lidar acquisition to compare surface elevation changes through time. We will use low resolution landsat, and possibly high resolution planet labs, imagery to track vegetation changes on the landslide scars through time. Then we will compare how these different changes may be correlated with spatial properties of the landslides, such as elevation, size, hillslope position, and aspect. 

## Expected outcomes
We hope to have a plot of how landslide scar surface elevation has changed through time on a small subset of landslides. We anticipate finding some areas of decreased elevation within landslide scars caused by reactivation in the form of debris flows. We also expect to find a signal of some vegetation recovery over the 8 years since the earthquake. It is unclear how these changes will be correlated with their spatial properties, though a correlation of vegetation recovery with aspect and an anticorrelation with elevation may be likely. 

## Any other relevant information, images/tables, references, etc.


## References

Massey, C., et al. "Landslides triggered by the 14 November 2016 M w 7.8 Kaikōura earthquake, New Zealand." Bulletin of the Seismological Society of America 108.3B (2018): 1630-1648.     
Pollock, W. (2020). A framework for regional scale quantitative landslide risk analysis. University of Washington.     
Grant, A., Wartman, J., & Abou-Jaoude, G. (2016). Multimodal method for coseismic landslide hazard assessment. Engineering Geology, 212, 146-160.     



