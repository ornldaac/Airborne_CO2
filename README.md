# Visualizing airborne in-situ CO<sub>2</sub> geotrajectory data from NetCDF using R

### Presented at 2022 Ecological Society of America workshop: *Exploring changes in vulnerable ecosystems with NASA data*

*Author: ORNL DAAC*  
*Date: August 16, 2022*  
*Contact for ORNL DAAC: uso@daac.ornl.gov*  

### Keywords: R, geotrajectory, airborne platform, CO2, NetCDF


# 1. Overview

This repository holds an exercise to demonstrate how to visualize airborne geotrajectory information saved in a NetCDF file and how to subset the dataset for further analysis.  The exercise uses the open-source software R.  The procedure is available as a R Markdown document for use with RStudio, in standard Markdown format, and as a PDF.

# 2. Dataset

## 2.1 ABoVE: Atmospheric Profiles of CO, CO2 and CH4 Concentrations from Arctic-CAP, 2017

This exercise will use data from *ABoVE_2017_insitu_10sec.nc*, a file downloaded from [Sweeney and McKain (2019)](https://doi.org/10.3334/ORNLDAAC/1658). The dataset includes measurements of carbon dioxide (CO<sub>2</sub>), methane (CH<sub>4</sub>), and carbon monoxide (CO) concentrations taken during flights over Alaska, Canada, and the continental U.S. in 2017. During the flights, air samples were collected and analyzed using on-board instrumentation. Each data point is a time-stamped measurement taken in 3-dimensional space (longtitude, latitude, altitude).  During 2017, the flight lines were repeated several times between April to November, with some spatial variability, in order to sample sample carbon dynamics over northern biomes during the growing season.

Please review the The [User Guide](https://daac.ornl.gov/ABOVE/guides/ABoVE_Arctic_CAP.html) for this dataset before starting the exercise.  This guide contains important information on the organization of the dataset and variables. It will be helpful to have the User Guide open for quick reference.

Sweeney, C., and K. McKain. 2019. ABoVE: Atmospheric Profiles of CO, CO2 and CH4 Concentrations from Arctic-CAP, 2017. ORNL DAAC, Oak Ridge, Tennessee, USA. <https://doi.org/10.3334/ORNLDAAC/1658>

## 2.2 Arctic-Boreal Vulnerability Experiment (ABoVE) project

The Arctic-Boreal Vulnerability Experiment (ABoVE) is a NASA Terrestrial Ecology Program field campaign based in Alaska and western Canada between 2016 and 2021. Research for ABoVE links field-based, process-level studies with geospatial data products derived from airborne and satellite sensors, providing a foundation for improving the analysis and modeling capabilities needed to understand and predict ecosystem responses and societal implications.

# 3. Prerequisites

Participants should have a basic understanding of R and some exposure to geospatial data and analysis.

## 3.1 R

1. [Download R](https://cran.r-project.org/)  
2. [Download RStudio](https://www.rstudio.com/products/rstudio/download/#download) - *Required* for R Markdown; *optional* for Markdown version 
3. These R packages must be installed: *ggplot2*, *lubridate*, *OpenStreetMap*, *RNetCDF*, *scales*, *sp*, *tmap*, and *tmaptools*. Code for installing these packages is included.   

## 3.2 Data

1. Sign in to [NASA Earthdata](https://urs.earthdata.nasa.gov/users/new). New users must set up an account in order to download data.  
2. Download [ABoVE_2017_insitu_10sec.nc](https://daac.ornl.gov/daacdata/above/ABoVE_Arctic_CAP/data/ABoVE_2017_insitu_10sec.nc)  
  

# 4. Procedure

## 4.1 Tutorial exercise  

1. [R Markdown](https://github.com/ornldaac/airborne_CO2/blob/main/Airborne_CO2_demo.Rmd)
2. [Markdown](https://github.com/ornldaac/airborne_CO2/blob/main/Airborne_CO2_demo.md)
3. [PDF](https://github.com/ornldaac/airborne_CO2/blob/main/Airborne_CO2_demo.pdf)

## 4.2 Additional resources

For users new to NetCDFs, these resources may be useful.

* [*NetCD-what? An Ecologist’s Guide to Working with Daymet and other NetCDF-formatted Data*](https://daac.ornl.gov/resources/tutorials/NetCDF_webinar_08302017.html) explains the NetCDF file format with examples from gridded weather data.
* [*Webinar: NetCDF Why and How: Creating Publication Quality NetCDF Datasets*](https://daac.ornl.gov/resources/tutorials/create_publication_quality_netcdf/) discusses the 'how and why' of using the NetCDF data structure 
*  [*How to Open and Work with NetCDF Data in R*](https://github.com/ornldaac/netCDF_data_in_R) is a tutorial providing additional practice working with this data format in R.

# 5. Credits  

* Klausner, T.,  M. Mertens, H. Huntrieser, M. Galkowski, G. Kuhlmann, R. Baumann, A. Fiehn, P. Jöckel, M. Pühl, A. Roiger. 2020. Urban greenhouse gas emissions from the Berlin area: A case study using airborne CO2 and CH4 in situ observations in summer 2018. Elementa: Science of the Anthropocene 8:15. https://doi.org/10.1525/elementa.411
* Krings, T., B. Neininger, K. Gerilowski, S. Krautwurst, M. Buchwitz, J.P. Burrows, C. Lindemann, T. Ruhtz, D. Schüttemeyer, and H. Bovensmann. 2018. Airborne remote sensing and in situ measurements of atmospheric CO2 to quantify point source emissions. Atmospheric Measurement Techniques 11:721–739. https://doi.org/10.5194/amt-11-721-2018
* Parazoo, N.C., R. Commane, S. Wofsy, C.D. Koven, C. Sweeney, D.M. Lawrence, J. Lindaas, R. Y.-W. Chang, and C.E. Miller. 2016. Detecting Regional Patterns of Changing CO2 Flux in Alaska. PNAS 113:7733-7738. https://doi.org/10.1073/pnas.1601085113
* [R](https://www.r-project.org/) - ver 4.2.1 (2022-08-02) -- "Funny-Looking Kid"  
* [RStudio](https://www.rstudio.com/products/rstudio/) - IDE and notebook construction  
* Sweeney, C., and K. McKain. 2019. ABoVE: Atmospheric Profiles of CO, CO2 and CH4 Concentrations from Arctic-CAP, 2017. ORNL DAAC, Oak Ridge, Tennessee, USA. https://doi.org/10.3334/ORNLDAAC/1658
