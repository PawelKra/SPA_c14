<template>
  <div id="mapContainer"></div>
</template>

<script>
import "leaflet/dist/leaflet.css";
import L from "leaflet";

export default {
  name: "LeafletMap",
  data() {
    return {
      map: null,
    };
  },
  mounted() {
    var cities = L.layerGroup();
    L.marker([50.087735, 19.882424])
      .bindPopup("LDB")
      .addTo(cities);
    var mbUrl =
      "https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token=pk.eyJ1IjoibWFwYm94IiwiYSI6ImNpejY4NXVycTA2emYycXBndHRqcmZ3N3gifQ.rJcFIG214AriISLbB6B5aw";

    var grayscale = L.tileLayer(mbUrl, {
      id: "mapbox/light-v9",
      tileSize: 512,
      zoomOffset: -1,
      attribution: "@authors OSM | LDB 2021",
    });
    this.map = L.map("mapContainer", {
      center: [50.087735, 19.882424],
      zoom: 9,
      layers: [grayscale, cities],
    });
    var baseLayers = {
      Grayscale: grayscale
    };
    var overlays = {
      LDB: cities,
    };

    L.control.layers(baseLayers, overlays).addTo(this.map);
  },
  beforeUnmount() {
    if (this.map) {
      this.map.remove();
    }
  },
};
</script>

<style scoped>
#mapContainer {
  width: 100%;
  height: 400px;
}
</style>
