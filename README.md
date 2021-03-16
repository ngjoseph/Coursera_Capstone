# The Battle of the Neighbourhoods

*Capstone project for the [IBM Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science?#courses).*

The aim of this project is to use a data driven approach to help in selecting a suitable location to open a new restaurant in Bengaluru, Karnataka. Although the city is a large and dense market with great potential, it is also highly competitive and establishing a profitable business requires excellent and methodical planning.

## Methodology
Create a grid of potential locations and evaluate each zone on different parameters including population density, real estate costs, level of competition and the presence of complementary businesses. Although this project mainly focuses on the dine-in side of the business, we will also give some consideration the potential of online deliveries.

## Tools
Several python packages were used for this project, including the following:
- [H3 Geospatial System](https://h3geo.org/) by Uber is used to generate the hexagonal grid.
- Pandas, GeoPandas, NumPy for data tabulation and manipulation
- GeoJSON, Shapely, GeoPy for geocoding and working with geospatial data
- Requests, BeautifulSoup4 for data scraping
- requests-cache, diskcache for caching API requests
- Folium for map visualizations
- Plotly, MatPlotLib for general data visualization
- SciKitLearn for machine learning algorithms

## Data Sources
- [Data{Meet} repository](https://github.com/datameet/Municipal_Spatial_Data) for ward level maps of Bangalore.
- [FourSquare Places API](https://developer.foursquare.com/) for Points of Interest data.
- [Nominatim](https://nominatim.openstreetmap.org/ui/search.html) for forward & reverse geocoding.
- [Zomato Bangalore Restaurants Dataset](https://www.kaggle.com/himanshupoddar/zomato-bangalore-restaurants) by [Himanshu Poddar](https://www.kaggle.com/himanshupoddar)
