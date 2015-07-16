# testing-geojson

Different methods to load and display geoJson map data, using Leaflet API (with or without MapBox) or Google Maps API

1) Leaflet-Mapbox featureLayer to load geojson files from directory OR remote server, works with L.control.layers
- Demo http://jackdougherty.github.io/testing-geojson/leaflet-mapbox-directory-remote.html
- based on example https://www.mapbox.com/mapbox.js/example/v1.0.0/geojson-marker-from-url/
- requires signing up for MapBox account and inserting token, free service up to 50,000 map views or users per month
- Mapbox "supercharges L.geoJson" with L.mapbox.featureLayer, which can load GeoJSON via AJAX, setFilter, and simplestyle-spec
- read more at https://www.mapbox.com/guides/master-web-map-layers/

*My problem*: While I can make regular Leaflet do a getJSON call for geojson files in same directory or remote, I can't figure out how to make this work with L.control.layers in methods below
 
Still working on this 
- http://jackdougherty.github.io/testing-geojson/leaflet-getjson-control-layer.html
 
Another strategy I considered:
    // download geojson and modify file: var borders = {...     and }; at end; change suffix to .js
    // Load file in header script above, add as geojson layer, declare as variable (for layer control), add styling, then add to map

2) Leaflet with jQuery getJSON call of geojson files in same directory
- Demo http://jackdougherty.github.io/testing-geojson/leaflet-getjson-directory.html
- based on tutorial: http://maptimeboston.github.io/leaflet-intro/
- requires adding jQuery into header script
- requires adding geojson files into directory (convert from KML, CSV, other formats with http://geojson.io)
- problem: cannot figure out how to initialize each layer as a variable to use this method with L.control.layers

3) Leaflet with jQuery getJSON call of geojson files on remote server
- Demo http://jackdougherty.github.io/testing-geojson/leaflet-getjson-remote.html
- sample source data: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- requires adding jQuery into header script
- remote server must be CORS enabled
- avoid http vs https mix errors; link to hosted web page must match source (in this case, http)
- based on Leaflet tutorial http://savaslabs.com/2015/05/18/mapping-geojson.html

4) Google map.data.loadGeoJson call to remote server
- Demo http://jackdougherty.github.io/testing-geojson/google-remote.html
- sample source data: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- remote server must be CORS enabled
- avoid http vs https mix errors; link to hosted web page must match source (in this case, http)
- based on Google example https://developers.google.com/maps/documentation/javascript/examples/layer-data-quakes




