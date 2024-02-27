# USGS Earthquake Visualization

## Background

I was tasked with creating an interactive visualization for the United States Geological Survey (USGS) earthquake dataset. The USGS collects extensive data on earthquakes worldwide but lacks an effective way to present it. This visualization aims to provide a meaningful display of earthquake data to educate the public and government organizations.

## Creating the Earthquake Visualization

To complete the visualization, I followed these steps:

1. **Obtaining the Dataset:**
   - I visited the [USGS GeoJSON Feed page](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) to select a dataset.
   - After choosing a dataset ("All Earthquakes from the Past 7 Days"), I retrieved the JSON data.

2. **Importing and Visualizing the Data:**
   - I utilized Leaflet to build a map plotting all earthquakes based on their longitude and latitude.
     - The magnitude of earthquakes was represented by marker size, and depth was indicated by marker color intensity.
     - I extracted earthquake depth as the third coordinate.
   - Each marker had a popup displaying additional earthquake details.
   - A legend was added to provide context for the map data.

## Code Citations

Adding a custom legend with a color scale:
(Found in lines 86-103 of logic.js file and lines 12-24 of style.css file)

https://leafletjs.com/examples/choropleth/

Add CircleMarkers to a Leaflet map using pointToLayer:
(Found in lines 40-41 of logic.js file)

https://leafletjs.com/examples/geojson/
