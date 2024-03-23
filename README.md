
# Crisis Mapping - Earthquake
The project involves the development of a robust and comprehensive spatial graphical database system to address the challenges
presented by earthquake disasters in India. This system will make use of
PostgreSQL as the backend database for the storage and management of
earthquake-related data, while QGIS will serve as the platform for geospatial
visualization and analysis.

### Problem statement:
Design and implement a spatial graphical database system for crisis mapping
of earthquake events in India, using PostgreSQL as the backend and QGIS for
visualization. The system should enable real-time data collection, storage,
retrieval, and geospatial analysis of earthquake-related information to aid
disaster response and recovery efforts.

### Methodology
1. Data Collection
- Seismic Data:

Source: Historical seismic data will be sourced from reputable databases such
as the Indian Meteorological Department (IMD) or international earthquake
databases.

Software: Python or the preferred programming language will be employed to
fetch and preprocess the seismic data, ensuring compatibility with subsequent
stages of the project.

- Geological Features:
  
Source: Geological features data, encompassing fault lines, tectonic plate
boundaries, and soil types, will be gathered from geological surveys or
relevant organizations.

Software: GIS software, specifically QGIS, will be utilized for the
visualization and analysis of geological features. This data will then be stored
in the PostgreSQL database using PostGIS, ensuring the spatial elements are
effectively managed for subsequent geospatial analysis.

2. Dataset
The datasets used in the project are:

i. Historical Data of Earthquakes: This is a collection of data from the past
10 years on earthquakes that have happened in India's regions.

ii. Lithology Dataset: This contains state wise data on the types of rock and
soil materials found at specific locations.

iii. Fault Tectonic Dataset: This contains statewise data on the location,
orientation, and attributes of faults within a specific geological region.

iv. Tectonic Framework: This contains statewise data on the geological and
tectonic features of a region. A tectonic framework dataset provides essential
information about the structural elements and tectonic history of an area,
aiding in the understanding of the Earth's crustal evolution and the distribution
of geological features.

3. Visualization on Map
- Historical Data of Earthquakes:
Load the earthquake data into QGIS as a point layer, with attributes such as
magnitude, location, depth, and time.
Apply a graduated symbol style based on the magnitude of earthquakes, using
different colors or sizes for varying magnitudes.
Use the time manager plugin to animate the earthquake occurrences over the
past 10 years, providing a temporal perspective.

- Lithology Dataset:
Load the lithology dataset as a polygon layer, where each polygon represents a
different type of rock or soil.
Apply a unique color or pattern to each rock type for easy differentiation.
Use transparency to allow visualization of overlapping lithological features.

- Fault Tectonic Dataset:
Load the fault dataset as a line layer, representing fault lines.
Style the faults based on attributes such as fault type or magnitude.
Apply arrows or symbols to indicate the orientation of faults.

- Tectonic Framework:
Load the tectonic framework dataset as a polygon layer, where each polygon
represents a different tectonic feature.
Style the tectonic features based on their types, such as plate boundaries,
volcanic regions, or fold structures.
Use transparency to allow visibility of multiple tectonic features.

- Integrated Visualization: 
Overlay the earthquake data, lithology, fault tectonic, and tectonic framework
layers to create a comprehensive map.
Adjust the layer order to ensure that important features are visible. 
Utilize labeling to display additional information, such as the names of regions
or geological features.

### Results
- Lithology layer: Polygons representing different rock and soil types for each Indian state.
![Lithology](https://github.com/SiddhiBehere/Crisis-Mapping-Earthquake/blob/main/Lithology.png)

- Tectonic Framework layer: Polygons showing geological and tectonic features. Differentiated by feature types like plate boundaries, volcanic regions, or fold structures.

![Tectonic framework](https://github.com/SiddhiBehere/Crisis-Mapping-Earthquake/blob/main/Tectonic%20Framework.png)

- Fault Tectonic layer: 

![Fault Tectonic](https://github.com/SiddhiBehere/Crisis-Mapping-Earthquake/blob/main/Fault%20tectonic.png)

- Earthquake:

![Earthquake](https://github.com/SiddhiBehere/Crisis-Mapping-Earthquake/blob/main/Earthquake.png)

- [Dashboard](https://github.com/SiddhiBehere/Crisis-Mapping-Earthquake/blob/main/Crisis%20Mapping%20-%20Earthquake.pbix)

### Future Scope
Although earthquakes can't be predicted but according to fault lines and tectonic
frameworks, we can say that there is a possibility of earthquakes in the drawn
zone (green polygons).

![Predictions](https://github.com/SiddhiBehere/Crisis-Mapping-Earthquake/blob/main/Predictions.png)

### Note
Data maybe limited due to it's unavailability.
