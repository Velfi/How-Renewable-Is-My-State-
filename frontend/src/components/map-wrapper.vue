<script>
/*
  Props:
    - mapId: the id that should be assigned to the DOM element the map will mount to
  Private variables/references:
    - $map: a reference to the leaflet map component
*/
import L from 'leaflet'

export default {
  props: ['mapId'],
  mounted () {
    this.$map = L.map(this.mapId).setView(new L.LatLng(39, -92), 4)
    L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 6,
      attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
    }).addTo(this.$map)
  }
}
</script>

<style lang="scss">
  .leaflet-container {
    height: 500px;
    width: 1000px;
  }
</style>

<template>
  <div :id="mapId" class="leaflet-map-wrapper"></div>
</template>
