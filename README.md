# testing-geojson

Different methods to load and display geoJson map data, using Leaflet API (with or without MapBox) or Google Maps API

1) Leaflet with jQuery getJSON call of geojson files in same directory
- Leaflet demo http://jackdougherty.github.io/testing-geojson/getjson-directory-leaflet.html
- based on tutorial: http://maptimeboston.github.io/leaflet-intro/
- requires adding jQuery into header script
- requires adding geojson files into directory (convert from KML, CSV, other formats with http://geojson.io)
- problem: cannot figure out how to initialize each layer as a variable to use this method with L.control.layers

2) working on this
http://jackdougherty.github.io/testing-geojson/external-leaflet.html

3) Leaflet with jQuery getJSON call of geojson files on remote server
- Leaflet demo http://jackdougherty.github.io/testing-geojson/remote-leaflet.html
- sample source data: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- requires adding jQuery into header script
- remote server must be CORS enabled
- avoid http vs https mix errors; link to hosted web page must match source (in this case, http)
- based on Leaflet tutorial http://savaslabs.com/2015/05/18/mapping-geojson.html

4) Problem: How do to Leaflet remote call and declare each layer as a variable, to use with L.control.layers?
Mapbox L.mapbox.featurelayer method
https://www.mapbox.com/mapbox.js/example/v1.0.0/geojson-marker-from-url/

5) Google map.data.loadGeoJson call to remote server
- Google demo http://jackdougherty.github.io/testing-geojson/remote-google.html
- sample source data: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- remote server must be CORS enabled
- avoid http vs https mix errors; link to hosted web page must match source (in this case, http)
- based on Google example https://developers.google.com/maps/documentation/javascript/examples/layer-data-quakes




