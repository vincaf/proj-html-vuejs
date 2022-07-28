<template>
  <div id="app">
    <HeaderWeb />
    <MainWeb />
    <FooterWeb />
  </div>
</template>

<script>
import HeaderWeb from './components/HeaderWeb.vue';
import MainWeb from './components/Main/MainWeb.vue';
import FooterWeb from './components/Footer/FooterWeb.vue';

export default {
  name: 'App',
  components: {
    HeaderWeb,
    MainWeb,
    FooterWeb,
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.container{
  max-width: 1200px;
}
</style>
