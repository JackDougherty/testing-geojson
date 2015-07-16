# testing-geojson

Different methods to load and display geoJson map layers, using Leaflet API or Google Maps API

1) jQuery getJSON call of geojson files in same directory
- Leaflet demo http://jackdougherty.github.io/testing-geojson/getjson-directory-leaflet.html
- based on tutorial: http://maptimeboston.github.io/leaflet-intro/
- requires adding jQuery into header script
- requires adding geojson files into directory (convert from KML, CSV, other formats with http://geojson.io)
- problem: cannot figure out how to initialize each layer as a variable to use this method with L.control.layers

1) working on this
http://jackdougherty.github.io/testing-geojson/external-leaflet.html

1) jQuery getJSON call of geojson files on remote server
- Leaflet demo http://jackdougherty.github.io/testing-geojson/remote-leaflet.html
- Google demo http://jackdougherty.github.io/testing-geojson/remote-google.html
- sample source data: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- requires adding jQuery into header script
- remote server must be CORS enabled
- avoid http vs https mix errors; link to hosted web page must match source (in this case, http)
- based on Leaflet tutorial http://savaslabs.com/2015/05/18/mapping-geojson.html
- based on Google example https://developers.google.com/maps/documentation/javascript/examples/layer-data-quakes



### loading geojson files from a remote url
- tutorial http://savaslabs.com/2015/05/18/mapping-geojson.html
- load geoJson from remote URL: 
- must have CORS enabled on remote server
- served over http, not https, to avoid mix error, since source data is http

### demo
Leaflet with jQuery 


Google Maps 





