# Land Cover Classification in Southern Santa Barbara County Using Decision Trees

### Overview
This project demonstrates the application of a decision tree classifier for land cover classification in Southern Santa Barbara County. Utilizing multi-spectral imagery and data on specific land cover types, we can understand how land cover changes over time. This method is particularly effective in studying the impacts of various environmental changes, such as urbanization, deforestation, and climate change.

### Objectives
The main objective is to classify a Landsat scene into four primary land cover types:
- Green vegetation
- Dry grass or soil
- Urban areas
- Water bodies
We achieve this by employing supervised classification techniques, specifically decision tree classifiers. These classifiers use training data to create a model that can predict land cover types based on spectral information from satellite images.

### Data and Tools
- Satellite Imagery: Landsat 5 Thematic Mapper scene from September 25, 2007, including bands 1, 2, 3, 4, 5, and 7
- Software and Libraries: We use R for processing and analyzing the data, with specific packages like sf, terra, rpart, rpart.plot, and tmap
- Training Data: Geospatial data of Southern Santa Barbara County and polygons representing training sites for the different land cover types

### Workflow
1. Data reparation
- Load and process Landsat data
- Crop and mask the data to focus on the study area
- Convert Landsat values to reflectance, ensuring accurate representation of the land cover

2. Land cover classification
- Extract reflectance values at specific training sites
- Develop a decision tree model using the rpart package
- Apply the trained model to classify the entire Landsat scene into different land cover types

3. Visualization and analysis
- Visualize the classified map using color codes for different land cover types
- Analyze the distribution and characteristics of each land cover type within the study area

