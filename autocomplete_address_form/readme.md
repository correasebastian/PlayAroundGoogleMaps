--tios de objetos devueltos por el sevicio de autocompletado

https://developers.google.com/places/supported_types

colombia boundaries viewport

viewport: Hd
Ma: yd
J: -66.851923
j: -79.05584699999997
__proto__: yd
Qa: Fd
J: -4.22711
j: 12.4584303

---------------
http://stackoverflow.com/questions/8282026/how-to-limit-google-autocomplete-results-to-city-and-country-only

function initialize() {

 var options = {
  types: ['(cities)'],
  componentRestrictions: {country: "us"}
 };

 var input = document.getElementById('searchTextField');
 var autocomplete = new google.maps.places.Autocomplete(input, options);
}

------------------


http://rustamagasanov.com/blog/2014/09/04/google-places-limit-autocomplete-results-to-cities-only/