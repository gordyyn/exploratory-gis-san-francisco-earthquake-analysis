# exploratory-gis-san-francisco-earthquake-analysis
Exploratory geospatial analysis of San Francisco's most vulnerable zones when an earthquake occurs. Looking at soft-story buildings and their relationship with population density and redlining, I look at patterns that have negatively shaped the city of San Francisco. Created using ArcGIS Pro, ArcGIS Online, and ArcPy for data processing and visualization.


# Seismic Hazard Zones and Soft-Story Vulnerability in San Francisco

**Author:** Gordon Yuan  
**Date:** December 2025  

<img width="891" height="692" alt="image" src="https://github.com/user-attachments/assets/1a080f76-c6b8-49c7-91e8-98894b6e5846" />

## 📊 Project Overview
In San Francisco, certain buildings, referred to as ‘soft-story’ buildings, are some of the most vulnerable properties in the city. These 
are buildings with weaker and more flexible ground floors, which would not be able to withstand lateral forces. They typically have 
multiple stories. Officially, according to the San Francisco city website, soft-story buildings are defined as ‘wood-frame structures, 
containing five or more residential units, having two or more stories over a 'soft' or 'weak' story, and permitted for construction prior 
to January 1, 1978.’ The most common type of soft-story buildings are Tier 3 properties, which have the lowest risk of endangerment. 
Tier 4 properties are the second most abundant, and are usually structurally dangerous due to being in liquefaction zones. Tier 2 
properties are the third most abundant, and are very high risk due to housing significant numbers of people. Tier 1 properties are 
very uncommon, but are the most dangerous due to the high human occupancy, usually being schools or large facilities.  
By looking at these soft-story properties, I wanted to see how they related to the other vulnerable areas in the city: liquefaction 
zones. These are places where there is an abundance of saturated sand and silt, and would turn liquid-like in times of an earthquake. 
Looking at the map above, there are many liquefaction and landslide zones in the city, mainly near the beaches, while some are in 
the middle of the city. These zones, highlighted in blue, are secretly very deadly.  
Using spatial analysis, I wanted to find the worst places to live in or be at during a major earthquake. By first identifying the soft-story 
properties that are in the liquefaction zones, I could then add a buffer of 200 meters to highlight the most dangerous areas citizens 
could be in, in case of a major earthquake. Interestingly, the worst zones, highlighted in red, are near the middle and northeast of the 
bay, where many of these soft-story properties cluster. Notably, these areas strongly align with the Marina District, which has 
historically experienced severe damage during major earthquakes. In case of a seismic event, avoid being in the areas in red, since 
there is a high chance of injury or death. Evacuation efforts also would be hindered because of collapsed buildings. In such a dense 
city, being in places not near a point, blue highlight, or red highlight, would drastically increase the chances of survival.  

**Dataset Sources**
[San Francisco GIS Catalog](https://data.sfgov.org/Housing-and-Buildings/Map-of-Soft-Story-Properties/jwdp-cqyc)
[data.gov Dataset Catalog](https://catalog.data.gov/dataset/tiger-line-shapefile-2022-county-san-francisco-county-ca-all-lines)
[USGS Faults Database](https://www.usgs.gov/programs/earthquake-hazards/faults)
[San Francisco GIS Catalog](https://data.sfgov.org/Geographic-Locations-and-Boundaries/Soil-Liquefaction-Hazard-Zone/i4t7-35u3/about_data)



## 🧰 Tools & Technologies

- ArcGIS Pro (map creation, layouts, symbology)  
- ArcGIS Online (optional sharing, StoryMap/Dashboard integration)  
- Shapefiles & File Geodatabases (spatial data management)  
- Cartography techniques (graduated colors, graduated symbols, inset maps, Albers equal-area projection)  

---
