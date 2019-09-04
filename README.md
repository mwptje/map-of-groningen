# map-of-groningen
## The neighbourhoods of Groningen

### Using Python and the folium mapping library to create an interactive map

This example shows how to convert a Shape file to a GEOJson format using the geopandas library and then plot an interactive map using the folium mapping library

**Geopandas**

- A geopandas dataframe is similar to a pandas dataframe with some addtional geospatial features:
  - Using the geopandas read_file method to import a Shape file into a geopandas dataframe
  - Store specfic geospatial figures as polygon's or point's (longitude and latitude pairs)
  - Convert one geo-coordinate system to another
  - Export to a GEOJson format
  - Methods to calculate a distance between two points or calculate an area of a polygon
- A geopandas dataframe has all the features of a pandas dataframe which makes it easy to manipulate

**Folium**

- The folium library has the Choropleth class which enables you to create an interactive map
- The map can have the following functionality:
  - zoom-in/zoom-out
  - color coding of intensities, for example showing the population density of a neighbourhood
    a lower population density having a lighter color or shade and higher population density showing
    as a darker color or shade
  - adding a title and a legend
- More examples can be found [here](https://nbviewer.jupyter.org/github/python-visualization/folium/tree/master/examples/)

Here we will be using a GEOJson file and a geopandas dataframe to plot the population densities by neighbourhood
