# Quantifying Temporal Land Cover Change Using *rioxarray*
### Claire Wang | 11/27/2020
#### My repository of final project of IDCE 30274 - Programming GIS. This project is about temporal analysis on land-cover change.

## Data Source
- Land cover data from [Clark Labs](https://clarklabs.org/aquaculture/). This site owns a public inventory of pond aquaculture and coastal habitats in Bangladesh, Cambodia, Ecuador, India, Indonesia, Malaysia, Myanmar, Thailand, and Vietnam. Landcover maps are in development for the years 1999, 2014, and 2018 for these countries. 
- [rioxarray](https://corteva.github.io/rioxarray/stable/) and [Rasterio](https://rasterio.readthedocs.io/en/latest/): Python libraries to calculate and plot raster dataset. Some [Turorials](https://carpentries-incubator.github.io/geospatial-python/aio/index.html) can be found here, along with tutorials of [Geopandas](https://geopandas.org/), the library for vector data.

## Motivations and Objectives
- The idea of time series is taken from a spatial statistics course: **Geog 379**. The Professor, Dr. Gil Pontius, spent some time discussing land change over time, and how the change could be quantified and visualized. I became very interested in analyzing land covers' temporal change, and developed a way to quantify change: **anything is classified as change except persistence** For example, if a pixel in category A 1. changes to category B; 2. changes to category C; 3. persists; 4. changes back to category B - across 4 time periods, this pixel will result in a value of 1+1+0+1 = 3. 
- It doesn't matter which category the pixel changes to, or if it changes back (toggle). As long as it experiences changes, it gains 1.
- This "metric" has insights in quantifying **sensitiveness/volatility** of the land cover, and can be further applied to remote sensing, conservation, and etc..

## 
