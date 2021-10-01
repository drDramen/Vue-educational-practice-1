<template>
  <div id="app">
    <div class="user-card">
      <CommonInfo
        :info="{
          name: user.name,
          username: user.username,
          email: user.email,
        }"
      />
      <ContactInfo :phone="user.phone" :website="user.website" />
      <Address :address="user.address" />
      <Company :company="user.company" />
    </div>
  </div>
</template>

<script>
import CommonInfo from '@/components/CommonInfo.vue';
import ContactInfo from '@/components/ContactInfo.vue';
import Address from '@/components/Address.vue';
import Company from '@/components/Company.vue';

export default {
  name: 'App',
  data: () => ({
    user: {
      id: 1,
      name: 'Leanne Graham',
      username: 'Bret',
      email: 'Sincere@april.biz',
      address: {
        street: 'Kulas Light',
        suite: 'Apt. 556',
        city: 'Gwenborough',
        zipcode: '92998-3874',
        geo: {
          lat: '-37.3159',
          lng: '81.1496',
        },
      },
      phone: '1-770-736-8031 x56442',
      website: 'hildegard.org',
      company: {
        name: 'Romaguera-Crona',
        catchPhrase: 'Multi-layered client-server neural-net',
        bs: 'harness real-time e-markets',
      },
    },
  }),
  methods: {},
  components: {
    CommonInfo,
    ContactInfo,
    Address,
    Company,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  padding: 0 50px;
}
.user-card {
  padding: 20px;
  width: 600px;
  border: 1px solid #000;
}
.card-row {
  display: flex;
}
.card-row > p {
  text-align: left;
}
.row-title {
  padding-right: 10px;
  min-width: 50%;
  font-weight: bold;
  text-align: right;
}
</style>
