<style>
#map {
  width: 500px;
  height: 500px;
  background-image: url('./map.jpg');
  position: relative;
}

.map-spot {
  width: 50px;
  height: 50px;
  border-radius: 25px;
  background-color: yellow;
  position: absolute;
  cursor: pointer;
}

#spot-1 {
  top: 100px;
  left: 100px;
}

#spot-2 {
  top: 200px;
  left: 300px;
}

#spot-3 {
  top: 350px;
  left: 200px;
}

#spot-4 {
  top: 400px;
  left: 50px;
}

#preview {
  width: 400px;
  height: 400px;
  background-image: url('./default.jpg');
  background-size: cover;
  margin: 50px auto;
  display: none;
}

</style>
  <head>
    <meta charset="UTF-8">
    <title>Interactive Map</title>
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>
  <body>
    <h1>Interactive Map</h1>
    <div id="map"></div>
    <div id="preview"></div>
    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY"></script>
    <script src="script.js"></script>
  </body>


<script>
    const locations = [
  {
    lat: 37.7749,
    lng: -122.4194,
    src: './san-francisco.jpg'
  },
  {
    lat: 40.7128,
    lng: -74.0060,
    src: './new-york.jpg'
  },
  {
    lat: 41.9028,
    lng: 12.4964,
    src: './rome.jpg'
  }
];

const preview = document.querySelector('#preview');

function initMap() {
  const map = new google.maps.Map(document.getElementById('map'), {
    zoom: 2,
    center: { lat: 0, lng: 0 }
  });

  locations.forEach(location => {
    const marker = new google.maps.Marker({
      position: location,
      map: map,
      title: 'Click to see a photo'
    });

    marker.addListener('click', () => {
      preview.style.backgroundImage = `url(${location.src})`;
      preview.style.display = 'block';
    });
  });
}

</script>

