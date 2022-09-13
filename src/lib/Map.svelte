<script>
  import L from 'leaflet'
  import '@geoman-io/leaflet-geoman-free'
  import '@geoman-io/leaflet-geoman-free/dist/leaflet-geoman.css'
  
  document.addEventListener("DOMContentLoaded", function() {
    map = L.map('map', {
      center: [31.998743, -80.847221],
      zoom: 15,  // EDIT from 1 (zoomed out) to 18 (zoomed in)
      scrollWheelZoom: true,
      tap: false
    });

    map.pm.addControls({
      position: 'topleft',
      drawCircle: false,
    });

    L.tileLayer(
      'https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}{r}.png', {
        attribution: '&copy; <a href="https://osm.org/copyright">\
          OpenStreetMap</a> contributors, &copy;\
          <a href="https://carto.com/attribution">CARTO</a>'
    }).addTo(map);
  })
</script>

<div class='fixed inset-y-0 left-0 right-0' id='map'></div>