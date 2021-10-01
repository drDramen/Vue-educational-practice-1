<template>
  <div>
    <p class="card-row">
      <span class="row-title">Company name (modified):</span>{{ nameModified }}
    </p>
    <p class="card-row"><span class="row-title">Catchphrase:</span>{{ company.catchPhrase }}</p>
  </div>
</template>

<script>
export default {
  name: 'Company',
  // props: ['info'],
  props: {
    company: Object,
  },
  data: () => ({}),
  computed: {
    nameModified() {
      return this.company.name.replace(' ', '-').toLowerCase();
    },
  },
};
</script>

<style></style>
