# The Battle of the Neighbourhoods

*Capstone project for the [IBM Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science?#courses).*

The aim of this project is to use a data driven approach to help in selecting a suitable location to open a new restaurant in Bengaluru, Karnataka. Although the city is a large and dense market with great potential, it is also highly competitive and establishing a profitable business requires methodical planning.

## Objective

Create a grid of potential locations and evaluate each zone on different parameters including population density, real estate costs, level of competition and the presence of complementary businesses.

## Guide

To run this notebook, the packages listed in **environment.yml** are required. In addition, certain notebooks require API keys (from FourSquare and HERE) to be stored as environment variables named as in the file.

The notebooks are intended to be viewed in order, as indicated by the numbering. View using [NBViewer](https://nbviewer.jupyter.org/) to load maps and interactive elements.

1. [Generating the H3 hexagonal grid](https://nbviewer.jupyter.org/github/ngjoseph/Coursera_Capstone/blob/main/notebooks/01_bangalore_grid_generation.ipynb)
2. [Reverse geocoding hexagon centers](https://nbviewer.jupyter.org/github/ngjoseph/Coursera_Capstone/blob/main/notebooks/02_bangalore_hex_addresses.ipynb)
3. [Scraping and interpolating real estate prices](https://nbviewer.jupyter.org/github/ngjoseph/Coursera_Capstone/blob/main/notebooks/03_bangalore_real_estate.ipynb)
4. [Obtaining Foursquare venue data](https://nbviewer.jupyter.org/github/ngjoseph/Coursera_Capstone/blob/main/notebooks/04_bangalore_foursquare_data.ipynb)
5. [Clustering Bangalore neighbourhoods](https://nbviewer.jupyter.org/github/ngjoseph/Coursera_Capstone/blob/main/notebooks/05_bangalore_clustering.ipynb)
6. [Evaluating and selecting locations](https://nbviewer.jupyter.org/github/ngjoseph/Coursera_Capstone/blob/main/notebooks/06_bangalore_location_selection.ipynb)

## Libraries

Several python libraries were used for this project, including the following:

- [H3 Geospatial System](https://h3geo.org/) by Uber to generate the hexagonal grid.
- Pandas, GeoPandas, NumPy for data tabulation and manipulation.
- GeoJSON, Shapely, GeoPy, Tobler for geocoding and working with geospatial data.
- Requests, BeautifulSoup4, Requests-cache, Diskcache for API calls, web scraping and caching data.
- Matplotlib, Plotly, Folium for data visualization and mapping.
- SciKitLearn for data scaling and clustering algorithms.

## Data Sources

- [Data{Meet} repository](https://github.com/datameet/Municipal_Spatial_Data) for ward level maps of Bangalore, including population statistics.
- [FourSquare Places API](https://developer.foursquare.com/) for Points of Interest data.
- [Nominatim](https://nominatim.openstreetmap.org/ui/search.html) and [HERE Geocoding & Search](https://www.here.com/platform/location-services/geocoding-and-search) for forward & reverse geocoding.
- [99Acres](https://www.99acres.com/property-rates-and-price-trends-in-bangalore) for real estate costs.
