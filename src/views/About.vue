<template>
  <div class="about">
    <GmapMap
      :center="{ lat: 32.158139, lng: 119.51325 }"
      :zoom="16"
      map-type-id="terrain"
      style="width:100%; height: 100vh"
    >
    </GmapMap>
  </div>
</template>
<script>
export default {
  name: "Home",
  methods: {},
};
</script>
