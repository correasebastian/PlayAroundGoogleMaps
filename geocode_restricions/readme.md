-- boundaries para medellin

var southwext={lat:6.1755969,long:-75.640916}//6.1755969,-75.640916
var northeast={lat:6.31281,long:-75.52150699999999}//6.31281,-75.52150699999999

J: -75.52150699999999
j: -75.640916
__proto__: yd
Qa: Fd
J: 6.1755969
j: 6.31281

---var auVicSwLatLon = new google.maps.LatLng(-39.234713, 140.962526);
var auVicNeLatLon = new google.maps.LatLng(-33.981125, 149.975296);
var auVicLatLonBounds = new google.maps.LatLngBounds(auVicSwLatLon, auVicNeLatLon);

bounds y componentrestriction funcionan bien independientemente

---
funciona inclusive mejor con ambas habilitadas

----

viewports and bounds

http://stackoverflow.com/questions/9491114/google-maps-api-v3-geocoder-results-issue-with-bounds

var resultBounds = new google.maps.LatLngBounds(

    results[0].geometry.viewport.getSouthWest(), 
    results[0].geometry.viewport.getNorthEast()
);

map.fitBounds(resultBounds);

----otro aproach para tratar de reducir la busqueda a solo posiciones que esten en una locacion

http://stackoverflow.com/questions/11847638/google-maps-api-geocoder-restricting-by-bounds