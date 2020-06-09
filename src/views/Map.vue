<template>
  <div id="map-canvas" style="width:100%;height:100vh;"></div>
</template>
<script>
// /*global google*/
export default {
  name: "Home",
  methods: {
    initialize() {
      const mapOptions = {
        zoom: 17,
        center: new google.maps.LatLng(32.158139, 119.51325),
      };
      const map = new google.maps.Map(
        document.getElementById("map-canvas"),
        mapOptions
      );
    },
  },
  mounted() {
    google.maps.event.addDomListener(window, "load", this.initialize);
  },
};
</script>
