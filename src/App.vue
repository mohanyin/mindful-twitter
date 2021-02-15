<template>
  <button @click="loginToTwitter">Log into Twitter</button>
</template>

<script lang="ts">
import axios from 'axios';

export default {
  methods: {
    loginToTwitter() {
      axios.get('http:localhost:3000/login/twitter');
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
