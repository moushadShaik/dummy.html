# dummy.html
<!DOCTYPE html>

<html>
  <head>
<style>

#map {
  height: 100%;
}


html,
body {
  height: 100%;
  margin: 0;
  padding: 0;
}

</style>
    <title>Simple Map</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=default"></script>
  
  </head>
  <body>
    <div id="map"></div>

 
    <script
      src="https://maps.googleapis.com/maps/api/js?key=AIzaSyB41DRUbKWJHPxaFjMAwdrzWzbVKartNGg&callback=initMap&v=weekly"
      defer
    ></script>
<script>

let map;

function initMap() {
  map = new google.maps.Map(document.getElementById("map"), {
    center: { lat: -34.397, lng: 150.644 },
    zoom: 8,
  });
}

window.initMap = initMap;
</script>
  </body>
</html>
