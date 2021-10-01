<template>
  <div>
    <p class="card-row"><span class="row-title">Geolocation:</span>{{ geo.lat}}, {{geo.lng}}</p>
    <p class="card-row"><span class="row-title">Geolocation JSON:</span>{{ toJson }}</p>
  </div>
</template>

<script>
export default {
  name: 'Geo',
  // props: ['info'],
  props: {
    geo: Object,
  },
  data: () => ({}),
  computed: {
    toJson() {
      return JSON.stringify(this.geo);
    },
  },
};
</script>

<style></style>
