# Land Cover Classification in Southern Santa Barbara County Using Decision Trees

### Overview
This repository details a project where decision tree classifiers are applied for systematic land cover mapping in Southern Santa Barbara County. The goal is to analyze land cover dynamics using Landsat 5 TM imagery, providing insights into environmental patterns and changes over time, such as urban expansion, vegetation changes, and water body distributions.

### Objectives
The central aim of this project is a detailed classification of a single Landsat scene, dated September 25, 2007, into four distinct land cover categories:
- Green vegetation
- Dry grass or soil
- Urban development
- Water bodies
This is accomplished through a supervised machine learning approach, leveraging the capabilities of decision tree classifiers that are informed by specific spectral signatures corresponding to each land cover type.

### Contents

### Repository Contents
```
├── data 
│ ├── landsat-data 
│ ├── trainingdata
│ └── SB_county_south
├── analysis.RMD
├── analysis.html
├── .RData
├── .Rhistory
├── README.md 
└── .gitignore
```


### Data and Tools
The project utilizes the following datasets and tools:
- Landsat Imagery: Landsat 5 TM scene encompassing bands 1-5 and 7, offering a comprehensive spectral view of the region
- Computational Tools: R is our chosen environment for data processing; sf, terra, rpart, rpart.plot, tmap
- Training Dataset: Defined by geospatial polygons that represent various land cover types, serving as a reference for our classification algorithm
Data are included in the .gitignore due to large size.

Data are stored in the .gitignore and can be accessed through this link: https://drive.google.com/file/d/1e9ZwWoC6kmqy5r7WtDOkabYa02jMx_sd/view

Landsat data: "Landsat 5." Landsat 5 \| U.S. Geological Survey. Accessed December 5, 2023. <https://www.usgs.gov/landsat-missions/landsat-5.>

Shapefile data: "Shapefiles." Shapefiles-ArcGIS \| Documentation. Accessed December 5, 2023. <https://doc.arcgis.com/en/arcgis-online/reference/shapefiles.htm.>

### Methodology
1. Data Preparation:
- Ingest and process the Landsat scene
- Crop and mask the imagery to our study area 
- Convert digital number values to reflectance for a true representation of surface characteristics

2. Classification Pipeline:
- Extract spectral data from known land cover training sites
- Construct and train a decision tree model to discern land cover types based on spectral data
- Apply the model across the Landsat scene, segmenting the landscape into the predefined categories

3. Visualization and Interpretation:
- Present the classification output 

