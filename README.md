# Using geospatial analyses to identify the impacts of extreme weather 

## Description
This repository is from an assignment completed in EDS 223 (Geospatial Analysis & Remote Sensing) at the Bren School of Environmental Science & Management. Through a series of geospatial analyses, it aimed to analyze the impacts of the severe 2021 winter storms in Houston, Texas. The frequency and intensity of extreme weather events are increasing due to climate change, bringing devastating impacts. In February 2021, the state of Texas suffered a major power crisis, which came about as a result of three severe winter storms sweeping across the United States on February 10–11, 13–17, and 15–20. This analysis identified the impacts of these extreme winter storms by estimating the number of homes that lost power throughout the Houston metropolitan area, and examining whether or not these impacts were distributed equitably across census tracts based on their median income levels.

## Repository organization description
```
├── scripts 
|   └── blackout_analysis_files
|       └── figure-HTML
|           └── fig-box-1.png            # boxplot of power outages (yes/no) by income level
|           └── fig-map1-1.png           # map of night light intensity pre- and post-storm
|           └── fig-map2-1.png           # map of homes that experienced blackouts 
|           └── fig-map3-1.png           # map of census tracts with power outages by income level
|       └── libs                         # other generated files from rendering the .qmd file
|   └── blackout_analysis.html           # FINAL REPORT, rendered html of the analysis 
|   └── blackout_analysis.qmd            # Quarto markdown doc used to generate the final report
├── .gitignore                           # files to ignore when pushing to GitHub 
├── README.md                            # description of repository
├── houston-blackout-analysis.Rproj      # R project file
```

## Skills

The repository demonstrates the following skills:

- loading and manipulating vector/raster data in R with the `sf` and `terra` packages
- conducting geospatial analyses in R
- simple vector and raster operations with `sf` and `terra`
- spatial joins
- creating maps in R with the `tmap` package
- creating a polished report in R using `quarto` 

## Data access
All relevant data available [here](https://drive.google.com/file/d/1bTk62xwOzBqWmmT791SbYbHxnCdjmBtw/view). Sourced from a shared course Google Drive, and imported into RStudio using the `here`, `sf`, and `terra` packages. 

The data was too large to upload to GitHub, but once downloaded, your repository should have the following structure:

```
houston-blackout-analysis
├── *folders/files listed above*
│
├──data
    │   gis_osm_buildings_a_free_1.gpkg
    │   gis_osm_roads_free_1.gpkg
    │
    └───ACS_2019_5YR_TRACT_48_TEXAS.gdb
    |   │   census tract gdb files
    |
    └───VNP46A1
    |   │   VIIRS data files
```

## Acknowledgements 
This assignment was created and organized Ruth Oliver, an Assistant Professor at the Bren School and the instructor for EDS 223. EDS 223 (Geospatial Analysis & Remote Sensing) is offered in the Masters of Environmental Data Science (MEDS) program at the Bren School. 

## References 
Wikipedia. 2021. “2021 Texas power crisis.” Last modified October 2, 2021. https://en.wikipedia.org/wiki/2021_Texas_power_crisis.
