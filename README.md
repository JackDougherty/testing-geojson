# testing-geojson

Different methods to load and display data as L.geoJson layers in Leaflet or Google Maps API

1) a jQuery getJSON call of geojson files in same directory in Leaflet
- demo http://jackdougherty.github.io/testing-geojson/getjson-directory-leaflet.html
- based on tutorial: http://maptimeboston.github.io/leaflet-intro/
- requires adding jQuery into header script
- problem: cannot figure out how to initialize each layer as a variable to use this method with L.control.layers

### demo
http://jackdougherty.github.io/testing-geojson/external-leaflet.html

Access remote geojson data or convert using http://geojson.io



### loading geojson files from a remote url
- tutorial http://savaslabs.com/2015/05/18/mapping-geojson.html
- load geoJson from remote URL: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- must have CORS enabled on remote server
- served over http, not https, to avoid mix error, since source data is http

### demo
Leaflet with jQuery 
http://jackdougherty.github.io/testing-geojson/remote-leaflet.html

Google Maps 
http://jackdougherty.github.io/testing-geojson/remote-google.html




