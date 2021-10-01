<template>
  <div>
    <p class="card-row"><span class="row-title">Full address:</span>{{ fullAddress }}</p>
    <Geo v-bind:geo="address.geo"></Geo>
  </div>
</template>

<script>
import Geo from '@/components/Geo.vue';

export default {
  name: 'Address',
  props: {
    address: Object,
  },
  data: () => ({}),
  components: {
    Geo,
  },
  computed: {
    fullAddress() {
      return `${this.address.zipcode}, ${this.address.city}, ${this.address.street}, ${this.address.suite}`;
    },
  },
};
</script>

<style></style>
