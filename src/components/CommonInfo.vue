<template>
  <div class="common-info">
    <p class="card-row"><span class="row-title">Name:</span>{{ info.name }}</p>
    <p class="card-row"><span class="row-title">Initials:</span>{{ initials }}</p>
    <p class="card-row"><span class="row-title">Nik:</span>{{ info.username }}</p>
    <p class="card-row"><span class="row-title">Email:</span>{{ info.email }}</p>
  </div>
</template>

<script>
export default {
  name: 'CommonInfo',
  props: ['info'],
  data: () => ({}),
  computed: {
    initials() {
      return this.info.name
        .split(/\s+/)
        .map((word) => `${word[0].toUpperCase()}.`)
        .join('');
    },
  },
};
</script>
