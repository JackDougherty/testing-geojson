# testing-geojson

## loading external geojson files in same directory
- tutorial: http://maptimeboston.github.io/leaflet-intro/
- load jQuery to create a simple function to call the data

### demo
http://jackdougherty.github.io/testing-geojson/external-leaflet.html

## loading geojson files from a remote url
- tutorial http://savaslabs.com/2015/05/18/mapping-geojson.html
- load geoJson from remote URL: http://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- must have CORS enabled on remote server
- served over http, not https, to avoid mix error, since source data is http

### demo
Leaflet with jQuery 
http://jackdougherty.github.io/testing-geojson/remote-leaflet.html

Google Maps 
http://jackdougherty.github.io/testing-geojson/remote-google.html




