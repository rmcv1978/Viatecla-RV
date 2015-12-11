# Viatecla-RV
Mapa

<!DOCTYPE html>
<html>
 <head>
   <title>Simple Map</title>
   <meta name="viewport" content="initial-scale=1.0">
   <meta charset="utf-8">
   <style>
     html, body {
       height: 100%;
       margin: 0;
       padding: 0;
     }
     #map {
       height: 100%;
     }
   </style>
 </head>
 <body>
   <div id="map"></div>
   <script>

var map;
function initMap() {
 var myLatLng = {lat: 38.7023593, lng: -9.1787769};

 var map = new google.maps.Map(document.getElementById('map'), {
   zoom: 12,
   center: myLatLng
 });

 var marker = new google.maps.Marker({
   position: myLatLng,
   map: map,
   title: 'Alphappl'
 });
}
   </script>
   <script src="https://maps.googleapis.com/maps/api/js?&callback=initMap"
       async defer></script>
 </body>
</html>
