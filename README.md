# NZLandslides

Paul added this... and now Luis added this... and Alan added this!


## Project Title:  

Ground Changes after Coseismic landslides in Kaikoura New Zealand

## Name(s) of individual or team members: 

Luis Angel Guerrero Hoyos, Paul Morgan, Alan Viola

## Short 1-2 sentence summary: 

This project aims to measure ground changes on landslide deposits after initial landsliding, and describe the factors that may have controlled these ground changes. 

## Some introductory background information: 
Recent landslide deposits and scars are commonly unstable often resulting in reactivation in the form of new landslides, or debris flows. These reactivations are a serious hazard often to already hard hit communities and infrastructure. In this project we aim to track landslide reactivations using Lidar DEM differencing and compare reactivations to metrics extracted from sattelite imagery and digital elevation models to estimate which landslide deposits may be most at rist for reactivation. For this we will use the Kaikour earthquake triggered landslides as case study.

On 14 November 2016, the region surrounding Kaikoura, New Zealand, experienced a M7.8 earthquake which triggered over 10,000 landslides. The modes of landsliding were diverse, including shallow, soil slides; rock avalanches and rock falls; and massive, deep-seated rotational slumps (Massey et al., 2018). Extensive mapping of the landslides triggered by the November 2016 earthquake has been undertaken by the New Zealand Institute of Geological and Nuclear Sciences (GNS) and Hakan Tanyas and coauthors(2022) who made their landslide polygon inventory publicly available.

Over the years, the GNS has done LiDAR and UAV - SfM surveys in the area that will serve as the main dataset to develop the project. The main goal is to track ground changes after the coseismic landslides, see how they’ve progressed over time, and find geospatial correlations between ground changes. We will focus on the LIDAR dataset collected by GNS between 2016 and 2019 and use the difference maps technique to identify the potential movements.


## Problem statement, question(s) and/or objective(s)

- Which landslides have been reactivated, and with what magnitude?
- Do landslide reactivations correlate with post-slide NDVI values?
- Do landslide reactivations correlate with slope/aspect/surface roughness of the landslide deposits?


## Datasets used (with links, if available)

Three Lidar DTMs from New Zealand Institute of Geological and Nuclear Sciences (GNS)
Landslide inventory polygon from GNS
Landsat 7, 8, and 9 collection 2 imagery
Planet labs imagery (hopeful)
Global SRTM DEM
Land Information New Zealand Data Service (LINZ) nation wide 8m DEM
https://data.linz.govt.nz/layer/51768-nz-8m-digital-elevation-model-2012/



## Tools/packages you’ll use (with links)
[Geopandas](https://github.com/geopandas/geopandas)
[Rasterio](https://github.com/rasterio/rasterio)
[rioxarray](https://github.com/corteva/rioxarray)
[numpy](https://github.com/numpy/numpy)
[matplotlib](https://github.com/matplotlib/matplotlib)
[odc.stac](https://github.com/opendatacube/odc-stac)
[gdal](https://github.com/OSGeo/gdal)
[pystac_client](https://github.com/stac-utils/pystac-client)
[planetary_computer](https://pypi.org/project/planetary-computer/)
[Whitebox geomorphometry](https://www.whiteboxgeo.com/)


## Overview of folders

### Notebooks
- NDVI_and_slidemovement - This script examines the relationship between landslide reactivation and NDVI
- NZ_slides_DEManalysis - This script runs through DEM analysis with the low resolution (8m) DEM from LINZ and the landslide inventory
- NZ_lidarareas - Code for analysis of Lidar DEMs and landslide data


## Methodology
For a small subset study area in the Kaikoura coast range we plan to compile several datasets to analyze what happens to landslides after they occur. We will gather several separate lidar acquisition to compare surface elevation changes through time. We will use low resolution landsat, and possibly high resolution planet labs, imagery to track vegetation changes on the landslide scars through time. Then we will compare how these different changes may be correlated with spatial properties of the landslides, such as elevation, size, hillslope position, and aspect. 

### DEM differencing


### NDVI analysis


### DEM analysis
Use of Whitebox geospatial to perform flow routing, roughness, slope, and aspect calculations. 


## General results outcomes

We found in general landslide scars experenced a decreasse in elevation from 2016 to 2018 with some landslide areas experienceing more changes than others.

We were able to map these landslide reactivation changes to a 2016 post earthquake NDVI measuret, and found that most of the large reactivation values occured on slide areas with small NDVI values(NDVI_and_slidemovement notebook). 

We also extracted slope roughness and aspect for these landslides, from the 2016 Lidar acuisistion, but found minimal correlations between these digital elevation metrics and reactivations (NZ_lidarareas notebook). 


## Future Work

- Run some type of landslide susceptibility code on the landslide deposit Lidar DEM to see if that correlates with reactivations. 
- Include many more DEM morphometry metrics

## Division of tasks

DEM analysis -Paul Morgan

## References


Tanyaş, Hakan, et al. "An open dataset for landslides triggered by the 2016 Mw 7.8 Kaikōura earthquake, New Zealand." Landslides 19.6 (2022): 1405-1420.

Massey, C., et al. "Landslides triggered by the 14 November 2016 M w 7.8 Kaikōura earthquake, New Zealand." Bulletin of the Seismological Society of America 108.3B (2018): 1630-1648.     

Pollock, W. (2020). A framework for regional scale quantitative landslide risk analysis. University of Washington.     

Grant, A., Wartman, J., & Abou-Jaoude, G. (2016). Multimodal method for coseismic landslide hazard assessment. Engineering Geology, 212, 146-160.     



