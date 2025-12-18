# exploratory-gis-san-francisco-earthquake-analysis
Exploratory geospatial analysis of San Francisco's most vulnerable zones when an earthquake occurs. Looking at soft-story buildings and their relationship with population density and redlining, I look at patterns that have negatively shaped the city of San Francisco. Created using ArcGIS Pro, ArcGIS Online, and ArcPy for data processing and visualization.


# Map 1

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
- [San Francisco GIS Catalog](https://data.sfgov.org/Housing-and-Buildings/Map-of-Soft-Story-Properties/jwdp-cqyc)
- [data.gov Dataset Catalog](https://catalog.data.gov/dataset/tiger-line-shapefile-2022-county-san-francisco-county-ca-all-lines)
- [USGS Faults Database](https://www.usgs.gov/programs/earthquake-hazards/faults)
- [San Francisco GIS Catalog](https://data.sfgov.org/Geographic-Locations-and-Boundaries/Soil-Liquefaction-Hazard-Zone/i4t7-35u3/about_data)

# Map 2

<img width="892" height="689" alt="image" src="https://github.com/user-attachments/assets/54edcbcc-d774-4d73-8cbb-39fc22ad0ac0" />

## 📊 Project Overview

This map examines the spatial relationship between soft-story building hot spots, historical redlining patterns, and present-day 
population density in San Francisco. By placing these variables side by side, the map shows how earthquake vulnerability is 
influenced not only by building characteristics, but also by historical and demographic factors. It is no coincidence that areas with the 
highest population density, lowest HOLC grades, and clusters of soft-story properties are all on top of each other.  
The left panel displays the results of a Getis-Ord Gi* hot spot analysis of soft-story buildings overlaid with Home Owners’ Loan 
Corporation (HOLC) redlining grades. According to the HOLC data source, ‘Green areas on the maps were called 'A,' 'First Grade,' or 
'Best' and were considered to be safest for loans. These areas were typically populated with wealthy, white residents that were born 
in the United States. Blue areas were called 'B,' 'Second Grade,' or 'Still Desirable.’ Yellow areas were called 'C,' 'Third Grade,' or 
'Definitely Declining.’ Red areas were called 'D,' 'Fourth Grade,' or 'Hazardous.’ HOLC recommended lenders refuse to make loans in 
these areas [or] only on a conservative basis.' These areas typically overlapped with Black and immigrant communities.’ The hot 
spots show clusters of cold spots or hot spots, where cold spots are clusters of less dangerous soft-story buildings (Tiers 3, 4) and hot 
spots are clusters of more dangerous soft-story buildings (Tiers 1, 2). Statistically significant hot spots are concentrated in the 
northeastern and central portions of the city, including areas such as the Marina, Mission District, and South of Market. Many of 
these hot spots overlap with neighborhoods that were historically graded C or D, which were subject to lower building standards.  
The right panel presents population density (2016) across San Francisco, revealing that several soft-story hot spot areas also contain 
high concentrations of residents. Neighborhoods such as the Mission and areas east of Twin Peaks exhibit both elevated population 
density and a high number of vulnerable structures. The Russian Hill, Nob Hill, and Chinatown in the northeast are also 
neighborhoods where population density, poor HOLC grades, and soft-story buildings overlap with each other.  

**Dataset Sources**
- [San Francisco GIS Catalog](https://data.sfgov.org/Housing-and-Buildings/Map-of-Soft-Story-Properties/jwdp-cqyc)
- [data.gov Dataset Catalog](https://catalog.data.gov/dataset/tiger-line-shapefile-2022-county-san-francisco-county-ca-all-lines)
- [ArcGIS Online](https://www.arcgis.com/home/item.html?id=d77c640241d84b6889ab290cd4cb755b)
- [ArcGIS Online](https://sigcfe.maps.arcgis.com/home/item.html?id=1bc6bc5a575846f38786db30bb3981e7)
- [USGS Faults Database](https://www.usgs.gov/programs/earthquake-hazards/faults)
- [ArcGIS Online](https://www.arcgis.com/home/item.html?id=0d64f2ffd1f54fe592f9aed107041c55)

# Map 3

<img width="898" height="693" alt="image" src="https://github.com/user-attachments/assets/ddb22b24-eb08-4f09-a23a-cda5bfffc494" />

## 📊 Project Overview
This final map looks at how emergency response coverage and transportation infrastructure are 
affected when earthquakes happen in San Francisco. By mapping fire stations, hospitals, BART 
infrastructure, highways, bridges, and seismic danger zones, the map shows how access and 
mobility can determine survival during and after a major earthquake. This spatial analysis 
emphasizes the importance of a strong transportation network and emergency systems in 
supporting evacuation and response efforts. 
During the 1989 Loma Prieta earthquake, San Francisco experienced extensive damage to 
highways and bridges, including the collapse of elevated freeway structures that severely 
disrupted transportation and emergency access. Bridges and highway interchanges built prior to 
modern seismic standards proved particularly vulnerable to ground shaking and liquefaction. In 
contrast, the Bay Area Rapid Transit (BART) system remained largely operational, with minimal structural damage, due to its seismic 
design features such as reinforced structures and flexible joints. The BART line was even able to run 24/7 during the disaster. This 
type of infrastructure allowed San Franciscoans to travel across the city without the use of cars.  
Fire stations are the lifelines of the city when a seismic event occurs, and should generally cover a half-mile radius in large cities. 
While much of the city falls within emergency service coverage, damaged bridges and highways could significantly delay response 
times or isolate neighborhoods following an earthquake. Fire stations that lie in liquefaction zones are vulnerable and may delay 
response. Areas with close proximity to BART stations may have greater mobility when surface transportation networks fail, 
emphasizing the role of resilient transit infrastructure in disaster response. 

**Dataset Sources**
- [data.gov Dataset Catalog](https://catalog.data.gov/dataset/tiger-line-shapefile-2022-county-san-francisco-county-ca-all-lines)
- [USGS Faults Database](https://www.usgs.gov/programs/earthquake-hazards/faults)
- [BART Geo Data](https://www.bart.gov/schedules/developers/geo)
- [ArcGIS Online](https://www.arcgis.com/home/item.html?id=89c8f080eafb41bb9e6c2f962c29a45b)
- [ArcGIS Online](https://www.arcgis.com/home/item.html?id=c66ea6559f5941a7a0cbcb98e72178e3)
- [San Francisco GIS Catalog](https://data.sfgov.org/Geographic-Locations-and-Boundaries/Soil-Liquefaction-Hazard-Zone/i4t7-35u3/about_data)



## 🧰 Tools & Technologies

- ArcGIS Pro (map creation, layouts, symbology)  
- ArcGIS Online (optional sharing, StoryMap/Dashboard integration)  
- Shapefiles & File Geodatabases (spatial data management)  
- Cartography techniques (graduated colors, graduated symbols, inset maps, Albers equal-area projection)  

---
