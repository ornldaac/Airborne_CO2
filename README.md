# Visualizing airborne, in-situ CO2 data from NetCDF using R

### *Presented at 2022 Ecological Society of America meeting* 

### *Workshop: Exploring changes in vulnerable ecosystems with NASA data*

### August 16, 2022


# 1. Overview

This repo hold an R Markdown document prepared for a workshop at the 2022 Ecological Society of America conference.

# 2. Dataset

This exercise will use data from *ABoVE_2017_insitu_10sec.nc*, a file downloaded from [Sweeney and McKain (2019)](https://doi.org/10.3334/ORNLDAAC/1658). The data set includes measurements of carbon dioxide (CO~2~), methane (CH~4~), and carbon monoxide (CO) concentrations taken during flights over Alaska, Canada, and the continental U.S. in 2017. During the flights, air samples were collected and analyzed using on-board instrumentation. Each data point is a time-stamped measurement taken in 3-dimensional space (longtitude, latitude, altitude).  During 2017, the flight lines were repeated several times between April to November, with some spatial variability, in order to sample sample carbon dynamics over northern biomes during the growing season.

Please review the The [User Guide](https://daac.ornl.gov/ABOVE/guides/ABoVE_Arctic_CAP.html) for this dataset before proceeding.  This guide contains important information on the organization of the dataset, file naming conventions, and variables. It will be helpful to have the User Guide open for quick reference.

Sweeney, C., and K. McKain. 2019. ABoVE: Atmospheric Profiles of CO, CO2 and CH4 Concentrations from Arctic-CAP, 2017. ORNL DAAC, Oak Ridge, Tennessee, USA. <https://doi.org/10.3334/ORNLDAAC/1658>

# 3. Prerequisites

Participants should have a basic understanding of R and some exposure to geospatial data and analysis.

## 3.1 R

1. [Download R](https://cran.r-project.org/)  
2. [Download RStudio](https://www.rstudio.com/products/rstudio/download/#download)  *Required for R Markdown; optional for Markdown version* 
3. These R packages must be installed: ggplot2, lubridate, OpenStreetMap, RNetCDF, sp, tmap, and tmaptools   

## 3.2 Data

1. [Sign in to NASA Earthdata](https://urs.earthdata.nasa.gov/users/new)  
2. [Download ABoVE_2017_insitu_10sec.nc](https://daac.ornl.gov/daacdata/above/ABoVE_Arctic_CAP/data/ABoVE_2017_insitu_10sec.nc)  
  

# 4. Procedure

## 4.1 Tutorial  

1. [R Markdown](https://github.com/jessnicwelch/edwebinar_mar19/blob/master/edwebinar_mar19_ornldaac_tutorial.Rmd)  
2. [Markdown](https://github.com/jessnicwelch/edwebinar_mar19/blob/master/edwebinar_mar19_ornldaac_tutorial.md)  

# 5. Credits

* [R](https://www.r-project.org/) - 4.1.0 (2021-05-18) -- "Camp Pontanezen"  
* [RStudio](https://www.rstudio.com/products/rstudio/) - IDE and notebook construction  
