<template>
  <div>
    <p class="card-row"><span class="row-title">Phone:</span>{{ phone }}</p>
    <p class="card-row"><span class="row-title">Short Phone:</span>{{ phoneShort }}</p>
    <p class="card-row"><span class="row-title">Website:</span>{{ website }}</p>
  </div>
</template>

<script>
export default {
  name: 'ContactInfo',
  props: {
    phone: String,
    website: String,
  },
  data: () => ({}),
  computed: {
    phoneShort() {
      return this.phone.replace(/\sx\d+/, '');
    },
  },
};
</script>

<style></style>
